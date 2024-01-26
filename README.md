# Multithreading---Overriding-start-method
class MyThread extends Thread
{
    public void start()
	{
	System.out.println("Start Method");
	}
	public void run()
	{
	System.out.println("Run Method");
	}
}
class Test
{
    public static void main(String[] args)
    {
     MyThread t = new MyThread();
     t.start();
     System.out.println("Main Method");
    }
}	
