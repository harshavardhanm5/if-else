# if-else

public class ClassA
{
    void meth1(int i)
	{
		System.out.println("-----meth1()---------");
		if(i<=10)
		{
			System.out.println("if block executed");
		}
		System.out.println("java is awesome");
		System.out.println("meth1() execution completed");
	}
	void meth2(int i)
	{
		System.out.println("-----meth2()-------");
		if(i<=10)
			System.out.println("if block executed");
			System.out.println("java is awesome");
			System.out.println("meth2() execution completed");
	}
	int meth3(int i)
	{
		System.out.println("-----meth3()------");
		if(i<=10)
			return 100;
			return 200;
	}
	void meth4(int i)
	{
		System.out.println("-----meth4()--------");
		if(true)
		{
			System.out.println("if block executed");
		}
		System.out.println("java is awesome");
		System.out.println("meth4() execution completed");
	}
	int meth5()
	{
		System.out.println("meth5() called");
		return 1;
	}
	int meth6()
	{
		System.out.println("meth6() called");
		return 99;
	}
	int meth7(int x,int y)
	{
		System.out.println("meth7() called");
		System.out.println("x:"+x);
		System.out.println("y:"+y);
		return 500;
	}
	void meth8(int i)
	{
		System.out.println("-----meth8()------");
		System.out.println("i value: "+i);
		
		ClassA obj=new ClassA();
		if(i<=obj.meth7(obj.meth5(),obj.meth6()))
		{
			System.out.println("if block exeuted");
		}
		else
		{
			System.out.println("else block executed");
		}
		System.out.println("java is awesome");
		System.out.println("meth8() execution completed");
	}
	void meth9(int i)
	{
		System.out.println("-----meth9()---------");
		if(i<=10)
		{
			System.out.println("if block executed");
		}
		else
			System.out.println("else block executed");
		System.out.println("java is awesome");
		System.out.println("meth9() execution completed");
	}
	void meth10(int i)
	{
		System.out.println("---------meth10()------------");
		if(i>0)
		{
			System.out.println(i+ "is a positive number");
			if(i%2==0)
				System.out.println(i+ "is even number");
			else
				System.out.println(i+ "is odd number");
		}
		else if(i<0)
		{
			System.out.println(i+"is a negative number");
		}
		else
			System.out.println(i+ " equal to 0");
		System.out.println("java is awesome");
		System.out.println("meth10() execution completed");
	}
	public static void main(String[] args)
	{
		ClassA aobj=new ClassA();
		aobj.meth1(100/50);
		aobj.meth2(100);
		System.out.println(aobj.meth3('A'-'B'+5));
		aobj.meth4(100);
		aobj.meth8(('A'*2)/2);
		aobj.meth9(50);
		aobj.meth10(0);
	}
}
