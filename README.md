# jobdevops
class One
{
	int a,b;
	void first(int x,int y)
	{
		a=x;
		b=y;
	}
	void display()
	{
		System.out.println("a =" + a + "b="+b);
	}
}
class Two extends One
{
	int a,b;
	void second(int x,int y)
	{	
		super.a=x;
		super.b=y;
	}
	void display()
	{
		super.display();
		System.out.println("a =" + a + "b="+b);
	}
}