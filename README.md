# AutomationProject
sept batch
11 sept

public class Sample1 {
	@AfterMethod
	public void s1() {
		System.out.println("login");
	}
	@Test(priority=3)
	public void a1() {
		System.out.println("TC01 run");
	}

	@Test(priority=1)
	public void a2() {
		System.out.println("TC02 run");
	}
	
	@Test(priority=2 , invocationCount=5)
	public void a3() {
		System.out.println("TC03 run");
	}
	@BeforeMethod
	public void Bmethod() {
		System.out.println("before method");
		
	}
}
