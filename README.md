# method1
test


import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;

public class Testing2 {

	public static void main(String[] args) throws InterruptedException {
		System.setProperty("webdriver.chrome.driver", "src/main/resources/chromedriver.exe");
		WebDriver driver = new ChromeDriver();
		driver.get("https://www.abhibus.com/?");
		driver.manage().window().maximize();
		
		Testing1 login = new Testing1(driver);
		login.login();
		
		Thread.sleep(5000);
		

		
	
		
		
		driver.quit();

	}

}
