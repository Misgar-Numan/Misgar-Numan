```c
#include <life.h>

#define GREETINGS "HELLO THERE 👋🏻"

// Defining my profile structure like a program because why not?
typedef struct {
    char* Name;         // The one and only
    char* DOB;          // Date of Birth (or as I like to call it, my annual upgrade)
    char* Location;     // Currently residing (not hiding, I promise)
    char* Host;         // My Educational Home
    char* Major;        // The thing I'm "majorly" trying to master
    struct {
        char* real[4];
        char* programming[3];
        char* computer[3];
    } Languages;
    char* Interests[3];
    struct {
        char* Instagram;
        char* Discord;
    } Connect;
} Profile;

void getProfileDetails(Profile* Me) {
    Me->Name = "Mohd Numan Asgar";
    Me->DOB = "2004-10-05";
    Me->Location = "Anantnag, Jammu and Kashmir";
    Me->Host = "SHMM Govt. Degree College Anantnag, University of Kashmir";
    Me->Major = "Computer Applications";

    // Real languages I speak (no, I don't speak emoji... yet)
    Me->Languages.real[0] = "English";  
    Me->Languages.real[1] = "Hindi";    
    Me->Languages.real[2] = "Urdu";      
    Me->Languages.real[3] = "Kashmiri";  

    // Programming languages (aka my secret languages that my friends don’t understand)
    Me->Languages.programming[0] = "C/C++";  
    Me->Languages.programming[1] = "JavaScript";  
    Me->Languages.programming[2] = "Python";  

    // Computer languages (the ones I write on my keyboard instead of speaking)
    Me->Languages.computer[0] = "HTML";  
    Me->Languages.computer[1] = "CSS";   
    Me->Languages.computer[2] = "Markdown";  

    // Interests that might make me sound cooler (or nerdier)
    Me->Interests[0] = "Programming";  
    Me->Interests[1] = "Gaming";  
    Me->Interests[2] = "Swimming";  

    // How to reach me in case you want to talk about programming or pizza
    Me->Connect.Instagram = "misgar_numan";
    Me->Connect.Discord = "misgar_numan";
}

int main() {
    Profile* Me = (Profile*)malloc(sizeof(Profile)); // Allocating space for my awesome self

    getProfileDetails(Me);

    // Here, we could add code to display my profile, but let’s keep it a mystery for now

    free(Me);  // Freeing up the space because even my memory needs a break!

    return 0;  // Ending the program, but not the fun!
}
```
