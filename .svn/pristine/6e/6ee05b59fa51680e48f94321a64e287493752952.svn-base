package functional.com.trailblazers.freewheelers;

import org.junit.AfterClass;
import org.junit.BeforeClass;
import org.junit.Test;
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.firefox.FirefoxDriver;

import static org.hamcrest.core.Is.is;
import static org.junit.Assert.assertThat;

public class HumansTxtTest {

    static WebDriver driver;

    @BeforeClass
    public static void before() {
        driver = new FirefoxDriver();
    }

    @AfterClass
    public static void after() {
        driver.close();
    }

    @Test
    public void shouldDisplayAllTheTeamMembers() {
        driver.get("http://localhost:8080/humans.txt");
        WebElement element = driver.findElement(By.tagName("pre"));
        String[] expectedTeamMembers = {"Nishitha Ningegowda",
                                        "Peter Gibbons",
                                        "Samir Nagheenanajar",
                                        "Michael Bolton",
				                        "Gabriela Zamudio",
					                    "Benazeer Khan",
                                        "Xiaojing Chen",
                                        "Thomas Morris",
                                        "Yvan Martin",
                                        "Aswathi Krishna Moorthy",
                                        "Raouf Aghrout",
                                        "Dixith Kumar",
                                        "Padma",
                                        "Saheli Ganguly",
                                        "Huang YunKun",
                                        "Geran Butcher",
                "Tao Jing",
                "Josh Howell"};
        assertThat(element.getText().split("\n"), is(expectedTeamMembers));
    }
}




