```
#include <iostream>
#include <string>

using namespace std;

struct Person
{
    char *firstname;
    char *lastname;
    string fullname = string(firstname) + " " + string(lastname);
    char *email;
    char *desc;
    struct social
    {
        char *github;
        char *linkedin;
        char *instagram;
    } social;
    struct skill
    {
        char *name;
    } skills[15];
};

int main()
{
    Person p;
    p.firstname = "Wahyu Cahyanto";
    p.lastname = "Bayu Agung";
    p.email = "wchynto.dev@gmail.com";
    p.desc = "I am a Informatics Engineering Student at the University of Trunojoyo Madura";

    // social
    p.social.github = "wchynto";
    p.social.linkedin = "wahyu-cahyanto-bayu-agung-54b61022a";
    p.social.instagram = "@wchynto.dev";

    // front-end
    p.skills[0]
        .name = "HTML";
    p.skills[1].name = "CSS";
    p.skills[2].name = "Javascript";
    p.skills[3].name = "Vue.js";

    // back-end
    p.skills[4].name = "PHP";
    p.skills[5].name = "Laravel";
    p.skills[6].name = "Node.js";
    p.skills[7].name = "Express.js";

    // database
    p.skills[8].name = "MySQL";
    p.skills[9].name = "MongoDB";

    // devops
    p.skills[10].name = "Git";
    p.skills[11].name = "Docker";
    p.skills[12].name = "Linux";
}

```
