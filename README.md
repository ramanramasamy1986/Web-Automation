package Steps;

import java.util.HashMap;
import java.util.Map;
import java.util.concurrent.TimeUnit;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;
import org.openqa.selenium.chrome.ChromeOptions;

import io.cucumber.java.en.*;
import io.github.bonigarcia.wdm.WebDriverManager;

public class COD  {

WebDriver driver= null;

@SuppressWarnings("deprecation")
@Given("open SSl Site")
public static void open_s_sl_site() throws Exception  {
	
	WebDriverManager.chromedriver().setup();
	
	Map<String, Object> prefs = new HashMap<String, Object>();


	prefs.put("profile.default_content_setting_values.notifications", 2);

	ChromeOptions options = new ChromeOptions();

	options.setExperimentalOption("prefs", prefs);

	
	ChromeDriver driver = new ChromeDriver(options);
	
	driver.get("https://adminuat4.shopper-stop.in/");
	driver.manage().window().maximize();
	driver.manage().timeouts().implicitlyWait(40, TimeUnit.SECONDS);
	Thread.sleep(4000);
    
}

@Given("Click on Login iCon")
public void click_on_login_i_con() {
	driver.findElement(By.xpath("(//i[@class='user-icon'])[1]")).click();
	

}

@When("Enter Email Id")
public void enter_email_id() {
	
}

@When("Enter Password")
public void enter_password() {
    // Write code here that turns the phrase above into concrete actions
    throw new io.cucumber.java.PendingException();
}

@When("click on login button")
public void click_on_login_button() {
    // Write code here that turns the phrase above into concrete actions
    throw new io.cucumber.java.PendingException();
}

@When("Click on brand banner from home page")
public void click_on_brand_banner_from_home_page() {
    // Write code here that turns the phrase above into concrete actions
    throw new io.cucumber.java.PendingException();
}

@When("Click on product in PLP page")
public void click_on_product_in_plp_page() {
    // Write code here that turns the phrase above into concrete actions
    throw new io.cucumber.java.PendingException();
}

@When("Select size in PDP page")
public void select_size_in_pdp_page() {
    // Write code here that turns the phrase above into concrete actions
    throw new io.cucumber.java.PendingException();
}

@When("Click on Add to bag button")
public void click_on_add_to_bag_button() {
    // Write code here that turns the phrase above into concrete actions
    throw new io.cucumber.java.PendingException();
}

@When("click on cart icon and navigate to cart page")
public void click_on_cart_icon_and_navigate_to_cart_page() {
    // Write code here that turns the phrase above into concrete actions
    throw new io.cucumber.java.PendingException();
}

@When("click on place order button")
public void click_on_place_order_button() {
    // Write code here that turns the phrase above into concrete actions
    throw new io.cucumber.java.PendingException();
}

@When("click on COD paymnet and order got placed")
public void click_on_cod_paymnet_and_order_got_placed() {
    // Write code here that turns the phrase above into concrete actions
    throw new io.cucumber.java.PendingException();
}

@Then("User can see order details on order summary page")
public void user_can_see_order_details_on_order_summary_page() {
    // Write code here that turns the phrase above into concrete actions
    throw new io.cucumber.java.PendingException();
}

@Given("I want to write a step with SSL")
public void i_want_to_write_a_step_with_ssl() {
    // Write code here that turns the phrase above into concrete actions
    throw new io.cucumber.java.PendingException();
}

@When("I check for the Order value in step")
public void i_check_for_the_order_value_in_step() {
    // Write code here that turns the phrase above into concrete actions
    throw new io.cucumber.java.PendingException();
}

@Then("I verify the Order status in step")
public void i_verify_the_order_status_in_step() {
    // Write code here that turns the phrase above into concrete actions
    throw new io.cucumber.java.PendingException();
}

		
	}

