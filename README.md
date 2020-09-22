<div align="center">

## C\+\+ Black Book, Chapter 6 \(Objects and Classes\)


</div>

### Description

If you already know the basics of C++, here is where to begin...
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[D/D\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/d-d.md)
**Level**          |Intermediate
**User Rating**    |3.8 (15 globes from 4 users)
**Compatibility**  |C\+\+ \(general\), Microsoft Visual C\+\+, Borland C\+\+
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__3-1.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/d-d-c-black-book-chapter-6-objects-and-classes__3-3067/archive/master.zip)





### Source Code

<P><FONT FACE="Verdana" SIZE="-1"><U><B><FONT COLOR="#000000">Objects and
		Classes </FONT></B></U></FONT></P>
	 <P><FONT FACE="Verdana" SIZE="-1">So far we know that structures are a way
		to put data elements together and functions organize the functionality of the
		program together. Now we will put both data elements and functions together
		with the use of classes.</FONT></P>
	 <P><FONT FACE="Verdana" SIZE="-1"> Lets say you are a scientist who wants
		to program a robot. This robot must have some characteristics and some
		functionality, so how do you give it one? </FONT></P>
	 <P><FONT FACE="Verdana" SIZE="-1" COLOR="#000000">The first thing we should
		do is creating a Class. A class has two parts: </FONT></P>
	 <P><FONT FACE="Verdana" SIZE="-1" COLOR="#FF0000">1. Attributes
		(Characteristics) <BR>2. Behaviors (Functionality) </FONT></P>
	 <P><FONT FACE="Verdana" SIZE="-1">In the attributes section you have to put
		your data members. In the behaviors section you have to put your member
		functions. Now we have a Robot.</FONT></P>
	 <P><FONT FACE="Verdana" SIZE="-1"> In order to create several of these
		robots, we need to create them in the form of objects. So each robot becomes an
		object and will carry similar attributes and behaviors. Also lets say one of
		the attributes of our robot is giving it a name and an age. This enables them
		to have different names and ages. </FONT></P>
	 <P><FONT FACE="Verdana" SIZE="-1">So here is how the class will look like:
		</FONT></P>
	 <P><FONT FACE="Verdana" SIZE="-1"><B>class</B> Robot <BR>{
		<BR><B>private:</B> char name[30]; <B>int</B> age; <BR><B>public:</B>
		Show_name(); <B>void</B> Set_info(); <BR>Robot(); /*this is called a
		constructor, it's job is to initialize data members and must have the same name
		as your class, I will talk about constructors in chapter 7*/<BR>} </FONT></P>
	 <P><FONT FACE="Verdana" SIZE="-1">//note that we are not passing any
		arguments to our functions, this is because the functions show_name() and
		Set_info() have direct access to our data members and are the members of the
		same class. <BR>Public means accessible from anywhere. /*also note that we set
		our data members as private, this is because we don't want any thing out side
		the class access them directly to make any changes to them. The only way we can
		change our data members is by using what we call accessor functions (like
		Show_name(); Set_info();) to modify or read our data members.*/</FONT></P>
	 <P><FONT FACE="Verdana" SIZE="-1"> <FONT>And this is how we implement our
		functions:</FONT></FONT></P>
	 <P><FONT FACE="Verdana" SIZE="-1"><FONT FACE="Verdana"
		SIZE="-1">Robot::Robot() //initializing our data
		members</FONT><BR>{<BR>strcpy(name," "); <BR>age=0;<BR>}</FONT></P>
	 <P><FONT FACE="Verdana" SIZE="-1"> <B>void</B> Robot::Set_info() /*:: this
		is a "Scope-resolution" which means that this function is from Robot class not
		any other class. Here we are modifying our data members*/<BR>{ <BR>cout&lt;&lt;
		"Enter name"; <BR>cin&gt;&gt;name; <BR>cout&lt;&lt; "Enter
		age";<BR>cin&gt;&gt;age; <BR>} </FONT></P>
	 <P><FONT FACE="Verdana" SIZE="-1">Robot::Show_name() <BR>{
		<BR><B>return</B> name;<BR>} </FONT></P>
	 <P><FONT FACE="Verdana" SIZE="-1">Now in main() we have to create our
		objects, so we say: </FONT></P>
	 <P><FONT FACE="Verdana" SIZE="-1"><B>void</B> main() <BR>{ <BR>Robot
		MachineRobot,CrappyRobot; //creating two objects of type Robot /*Note that we
		have used "Robot" to indicate that we are creating objects of this class type.
		*/ <BR>MachineRobot.Set_info(); //Get info for MachineRobot
		CrappyRobot.Set_info(); //Get info for CrappyRobot
		<BR>MachineRobot.Show_name(); //Display the name of this robot
		<BR>CrappyRobot.Show_name(); //Display the name of this robot <BR>} </FONT></P>
	 <P><FONT FACE="Verdana" SIZE="-1">So we used the accessor functions that we
		made to give our robots a name and an age. The output of the program will be:
		</FONT></P>
	 <P><FONT FACE="Verdana" SIZE="-1">Enter name: FirstRobot<BR>Enter age: 25
		<BR>Enter name: SecondRobot <BR>Enter age: 12 <BR>FirstRobot
		SecondRobot</FONT></P>
	 <P><I><FONT FACE="Verdana" SIZE="-1"> <B>To summerize: </B></FONT></I></P>
	 <P><FONT FACE="Verdana" SIZE="-1">We created a class that included certain
		attributes and certain behaviors. Then we created two object that carry with
		them the attributes and behaviors of that.</FONT></P>
	 <P><FONT FACE="Verdana" SIZE="-1">P.S You are welcome to ask any
		questions.</FONT></P>
	 <P><FONT FACE="Verdana" SIZE="-1">Pooya K. </FONT></P>
	 <P><FONT FACE="Verdana" SIZE="-1">Go ahead an search Google, the only place
		you will find my tutorial is on this site</FONT></P>
	 <P><FONT FACE="Verdana" SIZE="-1"></FONT></P>

