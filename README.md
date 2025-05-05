# cs201-film-homework-solved
**TO GET THIS SOLUTION VISIT:** [CS201 Film Homework Solved](https://www.ankitcodinghub.com/product/cs201-film-homework-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;100248&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS201  Film Homework  Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
In this homework, you will implement a film collection system to store the lead actor names of films in a particular collection. For each film, you will store its title, its director, its year, its duration and its list of lead actors. In your implementation, the collection of films and the list of lead actors in each film will need to be implemented using dynamically allocated arrays. The homework has two parts whose requirements are explained below.

PART A:

To take the final exam, you must submit this part and receive at least half of its points.

This part is a simplified version of the entire system. It stores the titles, directors, years and durations of films in a collection without their list of lead actors. The films will be stored in a dynamically allocated array of Film objects. Thus, you will first implement the Film class. This class is rather simple for Part A, but will need to be extended for Part B.

1. BelowistherequiredpartoftheFilmclass.ThenameoftheclassshouldbeFilm;theinterface for the class:

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>#ifndef __SIMPLE_FILM_H
#define __SIMPLE_FILM_H
</pre>
<pre>#include &lt;string&gt;
using namespace std;
#include &lt;iostream&gt;
</pre>
<pre>class Film{
public:
</pre>
Film(const string fTitle = “”, const string fDirector = “”, const unsigned int fYear = 0,

const unsigned int fDuration = 0);

<pre>   Film(const Film &amp;fToCopy);
   ~Film();
   void operator=(const Film &amp;right);
   string getTitle() const;
   string getDirector() const;
   unsigned int getYear() const;
   unsigned int getDuration() const;
</pre>
friend ostream&amp; operator&lt;&lt;(ostream&amp; out, const Film&amp; f);

<pre>private:
   string title;
   string director;
   unsigned int year;
   unsigned int duration;
</pre>
};

#endif

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
should be coded in a file called SimpleFilm.h and its implementation should be coded in a file called SimpleFilm.cpp.

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
<ul>
<li>The Film class should have the data members title, director, year, and duration (in minutes). You should implement get functions for these data members since they will be used to test your program.</li>
<li>You should also implement a default constructor that initializes the title, director, year, and duration data members. Additionally, you should implement your own copy constructor and destructor, and overload the assignment operator and the &lt;&lt; operator for outputting Film objects. Although you may use the default ones for some of these member functions, you are advised to implement them (although some may have no statements) in Part A so that it will be easier for you to extend them in Part B.</li>
<li>Do not delete or modify any part of the given data members or member functions. However, you may define additional data members and member functions, if necessary.</li>
</ul>
2. Below is the required part of the film collection (FC) class that you will code in Part A of this assignment. The name of the class should be FC; the interface for the class:

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>#ifndef __SIMPLE_FC_H
#define __SIMPLE_FC_H
</pre>
<pre>#include "SimpleFilm.h"
</pre>
<pre>class FC{
public:
</pre>
FC();

FC(const FC &amp;fcToCopy);

~FC();

void operator=(const FC &amp;right);

bool addFilm(const string fTitle, const string fDirector,

<pre>                const unsigned int fYear,
</pre>
const unsigned int fDuration);

bool removeFilm(const string fTitle, const string fDirector); unsigned int getFilms(Film *&amp;allFilms) const;

<pre>private:
   Film *films;
</pre>
<pre>   unsigned int noOfFilms;
</pre>
<pre>   unsigned int size;
};
</pre>
#endif

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
should be coded in a file called SimpleFC.h and its implementation should be coded in a file called SimpleFC.cpp.

<ul>
<li>Implement the default constructor, which creates an empty film collection. Also implement the copy constructor and destructor, and overload the assignment operator.</li>
<li>Implement the add and remove film functions whose details are given below:
Add a film: This function adds a film to the collection. The title, the director, the year, and the duration are specified as parameters. In this collection, the pair of title and director are unique (however, there can be multiple films with the same title and multiple films of the same director). Thus, if the user attempts to add a film with an already existing title and director, do not add the film and return false. Do not display any warning messages. Otherwise, if the film does not exist in the collection, add it to the collection and return true.

Remove a film: This function removes a film from the collection. The title and the director are specified as parameters. If the given film exists in the collection, remove it from the collection
</li>
</ul>
</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
and return true. Otherwise, if there is no film with the given title and director, do not perform any action and return false. Likewise, do not display any warning messages.

<ul>
<li>Implement the get function for films. The getFilms function should return the number of the films in the collection using the return value and the films in the collection by a pass-by- reference parameter called allFilms. Do not forget to put a deep copy of the films to the pass-by-reference parameter; otherwise, you may encounter run-time errors.</li>
<li>Do not delete or modify any part of the given data members or member functions. However, you may define additional functions and data members, if necessary.</li>
</ul>
3. TotestPartA,youshouldcodeyourownmainfunctioninaseparatefile.Donotforgettotestyour code for different cases. However, do not submit any file containing the main function; otherwise, you may lose a considerable number of points. We will code our own driver to grade Part A of your assignment. In doing that, we will use the get functions of the Film and FC classes. Thus, do not forget to implement the get functions of these two classes. Below is an example of the test code and its output. In this example code, there is a global function called displayAllFilms. We will use it to display the films in the collection and to understand whether you add/remove films correctly. If you want, you may use this global function for your tests as well. Notice that the last line of this global function is to deallocate the allFilms array. Do not remove this line if you get any run-time errors while using the function. If you have such run-time errors, most probably, you

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>#include "SimpleFilm.h"
#include "SimpleFC.h"
</pre>
void displayAllFilms(FC &amp;fc){

Film *allFilms;

unsigned int noOfFilms = fc.getFilms(allFilms);

cout &lt;&lt; “No of films: ” &lt;&lt; noOfFilms &lt;&lt; endl;

for (unsigned int i = 0; i &lt; noOfFilms; i++) cout &lt;&lt; allFilms[i];

<pre>   if (allFilms != NULL) delete [] allFilms;
}
</pre>
<pre>int main(){
   FC fc;
</pre>
fc.addFilm(“Midnight Cowboy”, “John Schlesinger”, 1969, 113); if (fc.addFilm(“Annie Hall”, “Woody Allen”, 1977, 93))

cout &lt;&lt; “Successful insertion of Annie Hall, 1977, ” &lt;&lt; “Woody Allen, 93 min” &lt;&lt; endl;

else

cout &lt;&lt; “Unsuccessful insertion of Annie Hall, 1977, ”

&lt;&lt; “Woody Allen, 93 min” &lt;&lt; endl;

fc.addFilm(“Full Metal Jacket”, “Stanley Kubrick”, 1987, 116); fc.addFilm(“Good Will Hunting”, “Gus Van Sant”, 1997, 126); fc.addFilm(“Requiem for a Dream”, “Darren Aronofsky”, 2000, 101); fc.addFilm(“The Diving Bell and the Butterfly”, “Julian Schnabel”,

2007, 112);

if (fc.removeFilm(“Zelig”, “Woody Allen”))

cout &lt;&lt; “Successful deletion of Zelig, Woody Allen” &lt;&lt; endl; else

cout &lt;&lt; “Unsuccessful deletion of Zelig, Woody Allen” &lt;&lt; endl; displayAllFilms(fc);

return 0; }

</div>
</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
made an error in implementing either the getFilms function or one or more of the destructor, copy constructor, and overloaded assignment operator.

The output should be:

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
Successful insertion of Annie Hall, 1977, Woody Allen, 93 min Unsuccessful deletion of Zelig, Woody Allen

No of films: 6

Midnight Cowboy, 1969, John Schlesinger, 113 min

Annie Hall, 1977, Woody Allen, 96 min

Full Metal Jacket, 1987, Stanley Kubrick, 116 min

Good Will Hunting, 1997, Gus Van Sant, 126 min

Requiem for a Dream, 2000, Darren Aronofsky, 101 min

The Diving Bell and the Butterfly, 2007, Julian Schnabel, 112 min

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
What to submit for Part A?

You should put your SimpleFilm.h, SimpleFilm.cpp, SimpleFC.h, and SimpleFC.cpp files into a folder and zip the folder. In this zip file, there should not be any file containing the main function. The name of this zip file needs to be:

PartA_secX_Firstname_Lastname_StudentID.zip

where X is your section number. Then you should follow the steps that are explained at the end of this document for the submission of Part A.

What to be careful about implementation and submission for Part A?

You need to read the “notes about implementation” and the “notes about submission” parts that are given at the end of this document.

</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
PART B:

Now, Part A is to be extended such that each film has a list of lead actors. The full functionality of this extended FC system is to be provided. In order for this to be done, the Film class needs to be extended such that it additionally keeps the list of lead actors contained. The lead actor list of a film must be kept in a dynamically allocated array of Actor objects. Note that the number of lead actors can be different from one film to another, but is normally fixed for a particular film. The details of the classes are given below.

1. TherequirementsoftheActorclassaregivenbelow.ThenameoftheclassshouldbeActor;its interface:

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>#ifndef __ACTOR_H
#define __ACTOR_H
</pre>
<pre>#include &lt;string&gt;
using namespace std;
#include &lt;iostream&gt;
</pre>
<pre>class Actor{
public:
</pre>
Actor(const string aName = “”, const string aBirthPlace = “”, const unsigned int aBirthYear = 0);

<pre>   Actor(const Actor &amp;actorToCopy);
   ~Actor();
   void operator=(const Actor &amp;right);
   string getName() const;
</pre>
<pre>   string getBirthPlace() const;
   unsigned int getBirthYear() const;
</pre>
friend ostream&amp; operator&lt;&lt;(ostream&amp; out, const Actor&amp; a);

<pre>private:
   string name;
</pre>
<pre>   string birthPlace;
</pre>
<pre>   unsigned int birthYear;
};
</pre>
#endif

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
should be coded in a file called Actor.h and its implementation should be coded in a file called Actor.cpp.

<ul>
<li>The Actor class keeps the name of an actor, her/his birth place and her/his birth year. The
name should be unique for each film. That is, a film cannot have multiple actors with the exact same name but different films may have an actor with the same name. You should implement get functions for the data members since they will be used to test your program.
</li>
<li>Implement your own default constructor, copy constructor, and destructor, and overload the assignment operator and the &lt;&lt; operator for outputting Actor objects.</li>
<li>Do not delete or modify any part of the given data members or member functions. However, you may define additional functions and data members, if necessary.</li>
</ul>
</div>
</div>
</div>
<div class="page" title="Page 6">
<div class="layoutArea">
<div class="column">
2. TherequirementsoftheFilmclassaregivenbelow.ThenameoftheclassshouldbeFilm.This time, the interface for the class:

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>#ifndef __FILM_H
#define __FILM_H
</pre>
<pre>#include "Actor.h"
</pre>
<pre>class Film{
public:
</pre>
Film(const string fTitle = “”, const string fDirector = “”, const unsigned int fYear = 0,

const unsigned int fDuration = 0);

Film(const Film &amp;fToCopy);

~Film();

void operator=(const Film &amp;right);

string getFilmTitle() const;

string getFilmDirector() const;

unsigned int getFilmYear() const;

unsigned int getFilmDuration() const;

unsigned int calculateAverageActorAge() const;

friend ostream&amp; operator&lt;&lt;(ostream&amp; out, const Film&amp; f);

<pre>private:
   string title;
   string director;
   unsigned int year;
   unsigned int duration;
   Actor *actors;
   unsigned int noOfActors;
   unsigned int size;
</pre>
};

#endif

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
should be coded in a file called Film.h and its implementation should be coded in a file called Film.cpp.

<ul>
<li>The Film class is similar to the one given in Part A. However, now it should keep a dynamic array of Actor objects as well. Similar to Part A, you should implement your own default constructor, copy constructor, and destructor, and do not forget to overload the assignment operator and the &lt;&lt; operator for outputting Film objects. Also, you should make sure to implement get functions for the title, director, year, and duration data members since they will be used to test your program.</li>
<li>Your class should have a public member function called calculateAverageActorAge which will be used for testing. This function should calculate the average age of the leading actors in the film upon which it is invoked and return it. Note that in implementing this function, you should consider the existence of films in which there are no actors.</li>
<li>Do not delete or modify any part of the given data members or member functions. However, you may define additional functions and data members, if necessary.</li>
</ul>
</div>
</div>
</div>
<div class="page" title="Page 7">
<div class="layoutArea">
<div class="column">
3. BelowistherequiredpartoftheFCclassthatyouwillcodeinPartBofthisassignment.Thename of the class should be FC; the interface for the class:

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>#ifndef __FC_H
#define __FC_H
</pre>
<pre>#include "Film.h"
</pre>
<pre>class FC{
public:
</pre>
FC();

FC(const FC &amp;fcToCopy);

~FC();

void operator=(const FC &amp;right);

bool addFilm(const string fTitle, const string fDirector,

<pre>                const unsigned int fYear,
</pre>
const unsigned int fDuration);

bool removeFilm(const string fTitle, const string fDirector); unsigned int getFilms(Film *&amp;allFilms) const;

bool addActor(const string fTitle, const string fDirector,

const string aName, const string aBirthPlace,

const unsigned int aBirthYear);

bool removeActors(const string fTitle, const string fDirector); unsigned int calculateAverageDuration() const;

<pre>private:
   Film *films;
</pre>
<pre>   unsigned int noOfFilms;
</pre>
<pre>   unsigned int size;
};
</pre>
#endif

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
should be coded in a file called FC.h and its implementation should be coded in a file called FC.cpp.

<ul>
<li>The FC class is similar to the one given in Part A. However, now it should also keep the list of leading actors for each film. Similar to Part A, you should implement your own default constructor, copy constructor, and destructor, and overload the assignment operator. Also you should make sure to implement the getFilms function, as explained before.</li>
<li>Implement the following functions that your extended system should support.
Add a film: This function adds a film to the collection. The title, the director, the year, and the duration are specified as parameters. In this function, the lead actor list is not specified; if there are any, lead actor(s) will be added later. In the film collection, the pair of title and director are unique (however, there can be multiple films with the same title and multiple films of the same director). Thus, if the user attempts to add a film with an already existing title and director, do not add the film and return false. Do not display any warning messages. Otherwise, if the film does not exist in the collection, add it to the collection and return true. This function is similar to what you will have implemented in Part A. But, in Part B, you should also create an empty lead actor list for the film when you add it to the collection.

Remove a film: This function removes a film from the collection. The title and the director are specified as parameters. If the given film exists in the collection, remove it from the collection and return true. Otherwise, if there is no film with the given title and director, do not perform any action and return false. Likewise, do not display any warning messages. Note that this function should also clear the lead actor list of the specified film. This function is similar to what
</li>
</ul>
</div>
</div>
</div>
<div class="page" title="Page 8">
<div class="layoutArea">
<div class="column">
you will have implemented in Part A. But now, for Part B, you should also remove the lead actor list when you remove the film from the collection.

Add a lead actor to the film: This function adds an actor to the lead actor list of a film in the collection. The title and the director of the film together with the name, the birth place, and the birth year of the actor are specified as parameters. In this function, you should take care of the following issues:

o If the specified film does not exist in the collection, do not perform any action and return false. Do not display any warning messages.

o All actor names are unique in a film. Thus, if the user attempts to add an actor with an existing name for the specified film, do not perform any action and return false. Do not display any warning messages. (However, different films may have an actor with the same name.)

o Otherwise, add the actor to the lead actor list of the specified film and return true.

Remove lead actor list from the film: This function clears the lead actor list of a film. The title and the director are given as parameters. If there is no film with the specified title and director, or if there are no actors in the lead actor list, do not perform any action and return false. Do not display any warning messages. Otherwise, clear the lead actor list of the specified film and return true.

Calculate the average duration of films in the collection: This function calculates the average duration of all films in the collection and returns the result. If there are no films in the collection, this function should return 0.

• Do not delete or modify any part of the given data members or member functions. However, you may define additional functions and data members, if necessary.

4. TotestPartB,youshouldcodeyourownmainfunctioninaseparatefile.Donotforgettotestyour code for different cases. However, do not submit any file containing the main function; otherwise, you may lose a considerable number of points. We will code our own driver to grade Part B of your assignment. In doing that, we will use the get functions of the Actor, Film, and FC classes. Thus, do not forget to implement the get functions of these three classes.

Below is an example of the test code and its output. In this example code, there are two global functions called displayAllFilms and displayStatistics. The former is the same as the one implemented for Part A. The purpose of the latter is to obtain some statistics about films. We will use these functions to understand whether you add/remove films and actor lists correctly. If you want, you may use these global functions for your tests as well. Again the last line is included to deallocate the allFilms array. Do not remove this line if you get any run-time errors while using these functions. If you have such run-time errors, most probably, you made an error in implementing either the getFilms function or one or more of the destructor, copy constructor, and overloaded assignment operator.

</div>
</div>
</div>
<div class="page" title="Page 9">
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>#include "Film.h"
#include "FC.h"
</pre>
void displayAllFilms(FC &amp;fc){

Film *allFilms;

unsigned int noOfFilms = fc.getFilms(allFilms);

cout &lt;&lt; “No of films: ” &lt;&lt; noOfFilms &lt;&lt; endl;

for (unsigned int i = 0; i &lt; noOfFilms; i++) cout &lt;&lt; allFilms[i];

<pre>   if (allFilms != NULL) delete [] allFilms;
}
</pre>
void displayStatistics(FC &amp;fc){

Film *allFilms;

unsigned int noOfFilms = fc.getFilms(allFilms);

if (allFilms != NULL) {

unsigned int count[11] = {0}, mins, age, totalAge,

<pre>                   noOfFilmsWithActors = noOfFilms;
</pre>
for (unsigned int i = 0; i &lt; noOfFilms; i++) { mins = allFilms[i].getFilmDuration();

if (mins &lt; 100) count[mins/10]++;

else count[10]++;

<pre>      }
      for (int i = 0; i &lt; 10; i++)
</pre>
<pre>          if (count[i] &gt; 0)
             cout &lt;&lt; "Number of films with duration in [ "
</pre>
<pre>                  &lt;&lt; i*10 &lt;&lt; "," &lt;&lt; (i+1)*10 &lt;&lt; ") min: "
</pre>
<pre>                  &lt;&lt; count[i] &lt;&lt; endl;
      if (count[10] &gt; 0)
</pre>
<pre>         cout &lt;&lt; "Number of films with duration &gt;= 100 min: "
              &lt;&lt; count[10] &lt;&lt; endl;
</pre>
cout &lt;&lt; “Average film duration: ”

&lt;&lt; fc.calculateAvgDuration(); &lt;&lt; ” min, ” &lt;&lt; endl;

<pre>      totalAge = 0;
      for (unsigned int i = 0; i &lt; noOfFilms; i++) {
</pre>
age = allFilms[i].calculateAverageActorAge(); if (age == 0) noOfFilmsWithActors–;

else totalAge += age;

<pre>      }
      if (noOfFilmsWithActors &gt; 0) {
</pre>
<pre>         age = totalAge/noOfFilmsWithActors;
</pre>
<pre>         cout &lt;&lt; "Average actor age: " &lt;&lt; age &lt;&lt; endl;
      }
</pre>
<pre>      delete [] allFilms;
   }
</pre>
}

</div>
</div>
</div>
</div>
<div class="page" title="Page 10">
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>int main(){
   FC fc;
</pre>
fc.addFilm(“Midnight Cowboy”, “John Schlesinger”, 1969, 113); fc.addActor(“Midnight Cowboy”, “John Schlesinger”,

“Jon Voight”, “Yonkers, NY, USA”, 1938); fc.addActor(“Midnight Cowboy”, “John Schlesinger”,

“Dustin Hoffman”, “Los Angeles, CA, USA”, 1937);

fc.addFilm(“Annie Hall”, “Woody Allen”, 1977, 96); fc.addActor(“Annie Hall”, “Woody Allen”,

“Woody Allen”, “Brooklyn, NY, USA”, 1935); fc.addActor(“Annie Hall”, “Woody Allen”,

“Diane Keaton”, “Los Angeles, CA, USA”, 1946);

fc.addFilm(“Full Metal Jacket”, “Stanley Kubrick”, 1987, 116); fc.addActor(“Full Metal Jacket”, “Stanley Kubrick”,

“Matthew Modine”, “Loma Linda, CA, USA”, 1959);

fc.addFilm(“Good Will Hunting”, “Gus Van Sant”, 1997, 126); fc.addActor(“Good Will Hunting”, “Gus Van Sant”,

<pre>               "Matt Damon", "Cambridge, MA, USA", 1970);
</pre>
fc.addFilm(“Requiem for a Dream”, “Darren Aronofsky”, 2000, 101); fc.addActor(“Requiem for a Dream”, “Darren Aronofsky”,

“Ellen Burstyn”, “Detroit, MI, USA”, 1932); fc.addActor(“Requiem for a Dream”, “Darren Aronofsky”,

“Jared Leto”, “Bossier City, LA, USA”, 1971);

fc.addFilm(“The Diving Bell and the Butterfly”, “Julian Schnabel”, 2007, 112);

fc.addActor(“The Diving Bell and the Butterfly”, “Julian Schnabel”, “Mathieu Amalric”,

“Neuilly-sur-Seine, France”, 1965); fc.removeFilm(“Full Metal Jacket”, “Stanley Kubrick”);

<pre>   displayAllFilms(fc);
   displayStatistics(fc);
</pre>
return 0; }

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
The output should be:

</div>
</div>
</div>
<div class="page" title="Page 11">
<div class="section">
<div class="layoutArea">
<div class="column">
No of films: 5

Midnight Cowboy, John Schlesinger, 1969, 113

<pre>   Jon Voight, Yonkers, NY, USA, 1938
</pre>
<pre>   Dustin Hoffman, Los Angeles, CA, USA, 1937
Annie Hall, Woody Allen, 1977, 96
</pre>
<pre>   Woody Allen, Brooklyn, NY, USA, 1935
</pre>
<pre>   Diane Keaton, Los Angeles, CA, USA, 1946
Good Will Hunting, Gus Van Sant, 1997, 126
</pre>
Matt Damon, Cambridge, MA, USA, 1970

Requiem for a Dream, Darren Aronofsky, 2000, 101

<pre>   Ellen Burstyn, Detroit, MI, USA, 1932
</pre>
Jared Leto, Bossier City, LA, USA, 1971

The Diving Bell and the Butterfly, Julian Schnabel, 2007, 112

Mathieu Amalric, Neuilly-sur-Seine, France, 1965 Number of films with duration in [ 90,100) minutes: 1 Number of films with duration &gt;= 100 minutes: 4 Average film duration: 109 min

Average actor age: 36

</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
What to submit for Part B?

You should put your Actor.h, Actor.cpp, Film.h, Film.cpp, FC.h, and FC.cpp files into a folder and zip the folder. In this zip file, there should not be any file containing the main function. The name of this zip file should be PartB_secX_Firstname_Lastname_StudentID.zip where X is your section number. Then you should follow the steps explained at the end of this document for the submission of Part B.

NOTES ABOUT IMPLEMENTATION (for both Part A and Part B):

</div>
</div>
<div class="layoutArea">
<div class="column">
1.

2. 3.

</div>
<div class="column">
You must use dynamically allocated arrays. You will receive no points if you use automatically allocated arrays, linked-lists or any other data structures such as vector/array from the standard library.

You are not allowed to use any global variables or any global functions when implementing the classes. However, you may use global functions to test your program, but should not submit them.

Your code must not have any memory leaks. You will lose points if your code has memory leaks even though it produces correct output. To detect memory leaks, you may want to use Valgrind which is available at http://valgrind.org.

</div>
</div>
<div class="layoutArea">
<div class="column">
NOTES ABOUT SUBMISSION (for both Part A and Part B):

<ol>
<li>ConformtotherulesgivenseparatelyforPartAandPartB.Thatis,thenameofclasses,thename of .h and .cpp files, and the name of zip files should conform to the specifications given separately for Part A and Part B. Otherwise, you may lose a considerable number of points.</li>
<li>Youneedtouploadtwozipfiles(oneforPartAandtheotherforPartB)usingtheuploadlink on Moodle (all sections) by the deadline. Read “what to submit for Part A” and “what to submit for Part B” sections very carefully.</li>
<li>No hardcopy submission is needed. The standard rules about late homework submissions apply. Late submissions need to be done by e-mailing your two zip files to your TA Ahmet Furkan Yıldırım.</li>
<li>Donotupload/e-mailanyfilescontainingthemainfunction.</li>
<li>You are free to code your programs on Linux or Windows platforms. However, we will test your
programs on “dijkstra.ug.bcc.bilkent.edu.tr” and we will expect your programs to compile and run on the dijkstra machine. If we cannot get your program to properly work on the dijkstra machine, you will end up losing a considerable number of points. Therefore, we recommend you to make sure that your program compiles and properly works on “dijkstra.ug.bcc.bilkent.edu.tr” before submitting your assignment.
</li>
<li>This assignment will be graded by your TA Ahmet Furkan Yıldırım (furkan.yildirim at bilkent edu tr). Thus, you may ask your homework related questions directly to him.</li>
</ol>
</div>
</div>
</div>
