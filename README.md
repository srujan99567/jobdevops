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
class Three extends Two
{
	int a,b;
	void third(int x,int y,int z,int z1,int z2,int z3)
	{
		super.a=z;
		super.b=z1;
		second(z2,z3);
		a=x;
		b=y;
	}
	void display()
	{
		super.display();
		System.out.println("a =" + a + "b="+b);
	}
}
