# Test_Automation
package org.sample;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;
import org.openqa.selenium.chrome.ChromeOptions;
import org.openqa.selenium.interactions.Actions;

public class Test_Amazon {

	public static void main(String[] args) throws InterruptedException {
		System.setProperty("webdriver.chrome.driver","C:\\Users\\ChandanaCS\\Downloads\\chromedriver-win64\\chromedriver-win64\\chromedriver.exe");
		
		WebDriver driver=new ChromeDriver();
		//div[@id='nav-tools']/a[2]
		driver.get("https://www.amazon.com/log-in/");
		driver.manage().window().maximize();
		
		//login 
		Thread.sleep(2000);
		driver.findElement(By.xpath("//span[text()='Account & Lists']")).click();
		
		driver.findElement(By.id("ap_email")).sendKeys("6360866647");
		
		driver.findElement(By.id("continue")).click();
		
		driver.findElement(By.id("ap_password")).sendKeys("Maheen@21");
		
		driver.findElement(By.id("signInSubmit")).click();
		
		//search tab
		Thread.sleep(2000);
		WebElement search=driver.findElement(By.id("twotabsearchtextbox"));
		search.sendKeys("iPhone");
		
		//lands on the 4th index of search menu
		Thread.sleep(2000);
		search.findElement(By.xpath("//div[@class='left-pane-results-container']/div[4]")).click();
		
		//select one element
		driver.findElement(By.xpath("//div[@class='a-section aok-relative s-image-fixed-height']/img[@src='https://m.media-amazon.com/images/I/71+txfM5+GL._AC_UY218_.jpg']")).click();
		
		//Add to list
		driver.findElement(By.id("add-to-wishlist-button-submit")).click();
		
		//view wishlist
		Thread.sleep(2000);
		driver.findElement(By.xpath("//a[text()='View Your List']")).click();	
		
		//add to cart
		Thread.sleep(2000);
		driver.findElement(By.xpath("//span[@class='a-button-inner']/a[@data-csa-c-item-id='B0CDPHCRWX']")).click();
		
		//view cart
		Thread.sleep(2000);
		driver.findElement(By.xpath("//span/a[@href='/gp/cart/view.html/ref=cm_wl_vc_lv']")).click();
		
		driver.findElement(By.id("a-autoid-0-announce")).click();
		
		driver.findElement(By.id("quantity_6")).click();
		
		Thread.sleep(2000);
		
		//mouse hover 
		Actions actions = new Actions(driver);
		WebElement subMenu=driver.findElement(By.xpath("//span[text()='Account & Lists']"));
		//To mouseover on sub menu
		actions.moveToElement(subMenu).build().perform();
		
		//sign out
		Thread.sleep(5000);
		driver.findElement(By.xpath("//span[text()='Sign Out']")).click();
		
		
		driver.close();
		
		
	}

}
