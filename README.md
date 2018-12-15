import java.io.BufferedReader;
import java.io.IOException;
import java.io.InputStreamReader;

public class LeapYear {
	public static void main(String[] args) throws IOException{
		int y;
		String  s, Leap;
		System.out.println("Please input a year:");
		BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
		s = br.readLine();
		y = Integer.parseInt(s);
			if ((y%4==0)&&(y%100!=0)||y%400==0) 
				Leap = " is";
			else 
				Leap = " is not";
			System.out.println (y + Leap + " Leap year");
	}

}
