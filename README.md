# cspackage lab_csw;
class A3{
	private String name;
	public A3(String name) {
		this.name= name;
		System.out.println("Objet created: "+name);
	}
	protected void finalise()throws Throwable{
		System.out.println("Garbage Collected: "+name);
	}
}
public class A4Q3 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
A3 obj= new A3("Object");
obj= null;
System.gc();
	}

}
w-codes
