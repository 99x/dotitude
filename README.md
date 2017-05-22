# .Net Workshop 2017 | University of Moratuwa - CSE 

The following documentation contains the information about the prerequisites for the *.Net Workshop 2017* and the Step-by-Step Guide to start developing the sample application that will be completed during the workshop. The students are required to Install the software and the tools mentioned in the **Prerequisites** section and Follow the **Step-by-Step Guideline** given below to partially complete the example application.

## Prerequisites
You must install the following software before the .Net Workshop

* Visual Studio 2015 Community Edition - [Download](https://www.microsoft.com/en-us/download/details.aspx?id=48146)



## Example Project

We will use an example project through out the .Net Workshop to explain the concepts and the techniques. It's is **mandatory** that you have the required software packages installed on your personal computers and follow the **Step-by-Step Guide** found bellow to start creating the example project. 

**You must:**
> complete the Example Project up to the point described in the Step-by-Step Guide to successfully follow along with the .Net Workshop agenda.
> The instructions are easy to understand and follow along.


# Step-by-Step Guide | Student Registration Application

## Step 01 - Creating The Application

Open Visual Studio 2015 Community Edition from the Start Menu or the Desktop Shortcut. Then, click on `File > New > Project` Menu Item. You will see the *New Project* dialog box where you can create a new Visual Studio Project.

There are a lot of project types to choose from, but for this Workshop we will focus on creating a **Windows Forms Application**. Select Windows Forms Application template under the `Visual C# > Windows` category on the left hand side of the New Project dialog.

>**Tip:**
> You can also search for installed templates by using the Search box on the top right corner of the New Project dialog box

After selecting the *Windows Forms Application* from the templates type in **StudentRegistration** as the *Name* of the project. Your screen should look something like this.

![New Project Dialog](https://github.com/kasunkv/UoM-CSE-DotNet-Workshop-2017/blob/master/Screenshots/1.png)

Click **OK** and create the project. After the project is created you will be presented with a screen similar to the screenshot bellow.

> **Note:**
> Don't worry if you are not familiar with the User Interface of Visual Studio. Most of the important aspects of Visual Studio will be covered during the workshop.

![New Project Dialog](https://github.com/kasunkv/UoM-CSE-DotNet-Workshop-2017/blob/master/Screenshots/2.png)

## Step 02 - Rename The Default Form

You can see the project structure on the *Solution Explorer* on the right hand side and `Form1.cs` file open in the left hand side of Visual Studio. Let's rename this Form1.cs file to a more meaning full name.

![New Project Dialog](https://github.com/kasunkv/UoM-CSE-DotNet-Workshop-2017/blob/master/Screenshots/3.png)

`Right Click` on the Form1.cs file on the Solution Explorer and select `Rename` on the menu that pops up. Then Rename `Form1.cs` to `MainForm.cs` and press Enter. You will be presented with a message box informing you about updating the references according to the filename change. See the image bellow

![New Project Dialog](https://github.com/kasunkv/UoM-CSE-DotNet-Workshop-2017/blob/master/Screenshots/4.png)

You need to accept the changes. Click on the **Yes** button to *automatically* do the reference updates. Now you will see that `Form1.cs` is renamed to `MainForm.cs`. 

Now let's make the form a little bit bigger. When you hover your mouse pointer on the bottom right corner of the form that is open your curser should change to a *double sided arrow*. Click and drag the form to make it a little bigger. You can make the form any size you like.

Now your screen should look something like this.

![New Project Dialog](https://github.com/kasunkv/UoM-CSE-DotNet-Workshop-2017/blob/master/Screenshots/5.png)


## Step 03 - Change Properties Of The MainForm

It's time to change some properties of the `MainFrom` or the Student Registration Application we are building. For this you need to select the MainForm on the designer, and then on the menu bar click on `View > Properties Window` to get the *Properties* window. See the screenshot below.

![New Project Dialog](https://github.com/kasunkv/UoM-CSE-DotNet-Workshop-2017/blob/master/Screenshots/6.png)

> **Tip:**
> You can also press `Ctrl + W` and then `Ctrl + P` keyboard combination to bring up the Properties Window

In the *Properties Window* you need to change the following Properties, to the given values.

* **Text** - *Student Registration*
* **StartPosition** - *CenterScreen*
* **ShowIcon** - *False*
* **MinimizeBox** - *False*
* **FormBorderStyle** - *FixedSingle*

>**Tip:**
>You can click on the property name in the *Properties Window* to see a small description of what that specific Property does.

See the screenshot below, You can see the Text Property of the MainForm is changed to *Student Registration*

![New Project Dialog](https://github.com/kasunkv/UoM-CSE-DotNet-Workshop-2017/blob/master/Screenshots/7.png)


## Step 04 - Add Initial User Interface Elements

It's time to add some User Interface elements to the *MainForm* of our application. To do that we need to open up the **Toolbox Windows** that contains all the User Interface elements supported for Windows Forms Application.

To bring up the *Toolbox* Windows, like we did for the Properties Window, on the Menu bar, click on `View > Toolbox` menu item. You will see a Toolbox Window pop up on the Visual Studio IDE.

![New Project Dialog](https://github.com/kasunkv/UoM-CSE-DotNet-Workshop-2017/blob/master/Screenshots/8.png)

> **Tip:**
> You can also press `Ctrl + W` and then `Ctrl + X` keyboard combination to bring up the Properties Window

First you need to add a *Label* to the MainForm of the application. Search for *Label* in the Toolbox by scrolling up/down and `Click and Drag` a Label on to the MainForm to place the label on the Form. You can drag and drop any where you like. 

Look at the screenshot below to see where to place the *Label*

![New Project Dialog](https://github.com/kasunkv/UoM-CSE-DotNet-Workshop-2017/blob/master/Screenshots/9.png)

> **Tip:**
> You can also *Search* for any UI element in the toolbox using the Search box on the top of the toolbox.

After dropping the label on to the *MainForm* change the `Text` Property of the *Label* from the *Properties Window* to *First name*. Now you can see the label has the First name text applied to it. Look at the screenshot below.

![New Project Dialog](https://github.com/kasunkv/UoM-CSE-DotNet-Workshop-2017/blob/master/Screenshots/10.png)

Then you need to add a `TextBox` to enter the First name. Search for *TextBox* in the *Properties Window* and drag and drop the `TextBox` on to the MainForm. You can resize it if you want. 

Next you need to change the **Name** Property of the `TextBox`. This *Name* property is used to get a reference (or to access the TextBox) from the C# code behind the MainForm. You will see this later.

Select the `TextBox` and Change the `Name` to *tbxFirstName* in the Properties Window. See the screenshot below.

![New Project Dialog](https://github.com/kasunkv/UoM-CSE-DotNet-Workshop-2017/blob/master/Screenshots/11.png)

Now, add one more `Label` and a `TextBox` to the MainForm for the Last name. Change the `Label` *Text* to *Last name* and change the *Name* of the `TextBox` to *tbxLastName*. 

You should get something similar to the below screenshot.

![New Project Dialog](https://github.com/kasunkv/UoM-CSE-DotNet-Workshop-2017/blob/master/Screenshots/12.png)


## Step 05 - Complete The Application User Interface

You need to add some more UI elements to the MainForm of our application.

First we need to add a `Button` to the MainForm to Add the Student details to a List. Search for `Button` on the *Toolbox* and drag and drop it on to the MainForm. 

>**Tip:**
>You can resize the `Button` by *hovering over the corner of the `Button` and click and dragging the corners*

You need to change 2 *Properties* of the `Button`. The *Text* of the `Button` to change what the `Button` displays and the *Name* of the `Button` to get a reference to it from the code behind.

Change the following properties to their corresponding values.

* **Text** - *Add Student*
* **Name** - *btnAdd*

See the screenshot below, You can see the *Text* of the `Button` is changed to *Add Student* and the *Name* of the `Button` is changed to *btnAdd*

![New Project Dialog](https://github.com/kasunkv/UoM-CSE-DotNet-Workshop-2017/blob/master/Screenshots/13.png)


Now it's time to add the List to display the names of the registered students. You need to add a `ListBox` for this.

Search for `ListBox` in the *Toolbox* window and drag and drop it on the MainForm. You can hover over the corners of the `ListBox` click and drag to resize the `ListBox`.

Change the *Name* Property of the `ListBox` from the Properties Window to get a reference to the `ListBox` from the code behind. Look at the screenshot below.

Change the following properties to their corresponding values.

* **Name** - *lstStudents*

![New Project Dialog](https://github.com/kasunkv/UoM-CSE-DotNet-Workshop-2017/blob/master/Screenshots/14.png)

Next you need to add 2 more `Button` to the MainForm to complete the User Interface for the Student Registration Application.

Search for `Button` on the *Toolbox*, drag and drop it on to the MainForm. Resize it and Place it where you like. This `Button` is to remove students from the `ListBox`. You need to change 2 Properties on the new `Button`.

Change the following properties to their corresponding values.

* **Text** - *Remove Student*
* **Name** - *btnRemoveStudents*

See the screenshot below,

![New Project Dialog](https://github.com/kasunkv/UoM-CSE-DotNet-Workshop-2017/blob/master/Screenshots/15.png)

Finally, add a `Button` to close the application. Drag and drip a `Button` to the MainForm. You need to also change 2 Properties on the `Button`

Change the following properties to their corresponding values.

* **Text** - *Close*
* **Name** - *btnClose*

See the screenshot below,

![New Project Dialog](https://github.com/kasunkv/UoM-CSE-DotNet-Workshop-2017/blob/master/Screenshots/16.png)


## Step 06 - Add The Code To Close The Application.

You are done with the changes to the MainForm in terms of the User Interface Elements. Now let's add a little bit of code to the application and **Run** the application to see everything is working properly.

Let's add code to close the application when you click on the *Close* `Button`. **Double Click** on the *Close* `Button` and you will be take to the *MainForm.cs* code View. This is the **Code Behind** file mentioned earlier. You can see that you are inside a method called `btnClose_Click`

This is the method associated with the `Click` *event* of the `Button`.

> **Note:**
> Don't worry, You will get to know more about Events, Code Behind files and many more during the .Net Workshop.

Let's add the code line that closes the application. Type in the following code line inside the `btnClose_Click` method.

```cs
this.Close();
```

When you are typing the code, Visual Studio IDE will provide some help to complete the code. See the screenshot below, 

![New Project Dialog](https://github.com/kasunkv/UoM-CSE-DotNet-Workshop-2017/blob/master/Screenshots/17.png)


Finally, the method should look something like this,

```cs
private void btnClose_Click(object sender, EventArgs e)
{
    this.Close();
}
```


## Step 07 - Run The Application

It's time to **Run** the application for the first time.

To *Run* the application, Click on the **Start** button on the Toolbar above with the *Green Play* icon. Look at the screenshot below,

![New Project Dialog](https://github.com/kasunkv/UoM-CSE-DotNet-Workshop-2017/blob/master/Screenshots/18.png)

After sometime, the application will start and you can try entering values to the `TextBox` for First and Last names and see. See the screenshot below,

![New Project Dialog](https://github.com/kasunkv/UoM-CSE-DotNet-Workshop-2017/blob/master/Screenshots/19.png)

> **Note**
> Right now the application does not do anything. But we will complete the application during the workshop.

Click on the Close button and see that the application exits and you should exit out of the *Debug* mode (Which, will be explained later).

### Congratulations, You have completed the Student Registration Application up to this point. 

### Please note that you are REQUIRED to complete the application to this point before you come to the .Net Workshop.

### The workshop will continue from this point onwards.

