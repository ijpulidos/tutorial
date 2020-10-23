ניתן [ לדלג מיד על החלק הזה](http://tutorial.djangogirls.org/en/installation/#install-python) אם אתם.ן לא משתמשים.ות בChromebook. אם כן, ההתקנה תהיה קצת שונה. באפשרותכן.ם להתעלם מהוראות ההתקנה אלו.

### Cloud IDE (PaizaCloud Cloud IDE, AWS Cloud9)

Cloud IDE הוא כלי שנותן לך עורך קוד וגישה למחשב הרץ על האינטרנט שעליו ניתן להוריד, לכתוב, ולהריץ תוכנות. במהלך המדריך, Cloud IDE ישמש כ*מחשב המקומי* שלך. עדיין תריצ.י פקודות בממשק הטרמינל בדיוק כמו שאר חבריך לכיתה בOS X, Ubuntu או Windows, אבל הטרמינל יהיה מחובר למחשב שפועל במקום אחר שcloud IDE מסדר בשבילך. הנה ההוראות לcloud IDEs (PaizaCloud Cloud IDE, AWS Cloud9). ניתן לבחור אחד מהcloud IDEs, ולעקוב אחר ההוראות של הcloud IDEs.

#### PaizaCloud Cloud IDE

1. לכו ל [PaizaCloud Cloud IDE](https://paiza.cloud/)
2. הירשמו ליצירת חשבון
3. לחצו *שרת חדש* ובחרו באפליקציית הDjango
4. לחצו על כפתור הטרמינל (בצד שמאל של החלון)

Now you should see an interface with a sidebar, buttons at the left. Click "Terminal" button to open terminal window with prompt like this:

{% filename %}Terminal{% endfilename %}

    $
    

The terminal on the PaizaCloud Cloud IDE is prepared for your instructions. You can resize or maximize that window to make it a bit bigger.

#### AWS Cloud9

Currently Cloud 9 requires you to sign up with AWS and enter credit card information.

1. Install Cloud 9 from the [Chrome web store](https://chrome.google.com/webstore/detail/cloud9/nbdmccoknlfggadpfkmcpnamfnbkmkcp)
2. Go to [c9.io](https://c9.io) and click *Get started with AWS Cloud9*
3. Sign up for an AWS account (requires credit card information, but you can use it for free)
4. In the AWS Dashboard, enter *Cloud9* in the search bar and click it
5. In the Cloud 9 dashboard, click *Create environment*
6. Name it *django-girls*
7. While configuring settings, select *Create a new instance for environment (EC2)* for "Environment Type" and the *t2.micro* "Instance type" (it should say "Free-tier eligible."). The default cost-saving setting is fine and you can keep the other defaults.
8. Click *Next step*
9. Click *Create environment*

Now you should see an interface with a sidebar, a big main window with some text, and a small window at the bottom that looks something like this:

{% filename %}bash{% endfilename %}

    yourusername:~/workspace $
    

This bottom area is your terminal. You can use the terminal to send instructions to the remote Cloud 9 computer. You can resize that window to make it a bit bigger.

### סביבה וירטואלית

A virtual environment (also called a virtualenv) is like a private box we can stuff useful computer code into for a project we're working on. We use them to keep the various bits of code we want for our various projects separate so things don't get mixed up between projects.

Run:

{% filename %}Cloud 9{% endfilename %}

    mkdir djangogirls
    cd djangogirls
    python3.6 -mvenv myvenv
    source myvenv/bin/activate
    pip install django~={{ book.django_version }}
    

(note that on the last line we use a tilde followed by an equal sign: `~=`).

### GitHub

צרו חשבון [GitHub](https://github.com).

### PythonAnywhere

The Django Girls tutorial includes a section on what is called Deployment, which is the process of taking the code that powers your new web application and moving it to a publicly accessible computer (called a server) so other people can see your work.

This part is a little odd when doing the tutorial on a Chromebook since we're already using a computer that is on the Internet (as opposed to, say, a laptop). However, it's still useful, as we can think of our Cloud 9 workspace as a place for our "in progress" work and Python Anywhere as a place to show off our stuff as it becomes more complete.

Thus, sign up for a new Python Anywhere account at [www.pythonanywhere.com](https://www.pythonanywhere.com).