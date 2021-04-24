
import java.util.InputMismatchException;
import java.util.Scanner;
public class QuizBee 
{
	public static void main(String[] args) 
	{
		
		takeTest();
		
		}
		
	static void takeTest()
	{
		
		String question[] = new String[10];
		question[0] = "1. What is the process of planning and creating a program? "
						+ "\n   (a)Programming (b) Command (c) Syntax";
		question[1] = "2. What is the problem-solving technique used in solving programming problems? "
						+ "\n   (a)Programming (b) Algorithm (c) Command";
		question[2] = "3. What is the method of describing computer algorithms using a combination of"
						+ " natural language and programming language?"
						+ "\n   (a)Programming (b) Algorithm (c) Pseudocode";
		question[3] = "4. What is the visual representation of an algorithm?"
	    				+ "\n   (a) Programming (b) Algorithm (c) Flowchart";
		question[4] = "5. What are the errors that might be encountered during the process of translation?"
						+ "\n   (a) Programming (b) Logical Errors (c) Syntax Errors";
		question[5] = "6. What are the errors that occur when the syntax of the program is correct, but"
						+ "the expected output is not?"
						+ "\n   (a) Programming (b) Logical Errors (c) Syntax Errors";
		question[6] = "7. What is the process of locating and correcting errors of a program?"
						+ "\n   (a) Programming (b) Syntax (c) Debugging";
		question[7] = "8. What is the language that the computer can directly understand?"
						+ "\n   (a) Programming (b) Assembly Language (c) Machine Language";
		question[8] = "9. What is the symbolic form of machine language that is easier for people to read?"
						+ "\n   (a) Programing (b) Assembly Language (c) Machine Langugage";
		question[9] = "10. What is a program that translates assembly language instructions into machine language?"
						+ "\n   (a) Programming (b) Assembly Language (c) Assembler";
		String correctAnswer[] = { "a","b","c","c","c","b","c","c","b","c"};
		
		Scanner scan = new Scanner(System.in);
		int score = 0;
		String answer;
		try
		{
		for(byte index = 0; index < question.length; index++)
		{
			System.out.println(question[index]);
			answer = scan.nextLine().toLowerCase();
			if(answer.equals(correctAnswer[index]))
			{
				score++;
			}
			else if(answer.equals(" "))
			{
				System.out.println("Cannot have a blank answer. Try again.");
			}
			else if(answer != "a" || answer != "b" || answer != "c")
			{
				throw new InvalidLetterException("Invalid Letter. Try again");
			}
			
		}
		System.out.println("You got " + score + " / 10");
		}
		catch(InputMismatchException ex)
		{
			System.out.println("Invalid Input. Try again.");
		}
		catch(InvalidLetterException ex)
		{
			System.out.println(ex.getMessage());
		}
	}	
				
}
class InvalidLetterException extends Exception
{
	public InvalidLetterException(String s)
	{
		super(s);
	}
}
		
