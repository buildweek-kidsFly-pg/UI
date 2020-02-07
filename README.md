UI by Adrian Nasaruk

github-pages: https://buildweek-kidsfly-pg.github.io/UI/

Created a "Home" and "About" page.

HTML for the Home-Page:
Head: <head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>KidsFly</title>
  <link href="https://fonts.googleapis.com/css?family=Comfortaa&display=swap" rel="stylesheet">
  <link href="CSS/index.css" rel="stylesheet">
</head>

Head for the About page:
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>About Us</title>
  <link href="https://fonts.googleapis.com/css?family=Comfortaa&display=swap" rel="stylesheet">
  <link href="CSS/index.css" rel="stylesheet">
</head>

Part of the HTML body:

navigation and header: <div class= "container">    
<div class = "headline">
    <div class = "logo">
        <img src="Images/kidsfly1.png" alt= "our logo">
    </div>
    <div class = "title">
        <h1>KidsFly!</h1>
    </div>
    <div class = "navigation">
        <a href= "index.html">Home</a>
        <a href= "about.html">About Us</a>
    </div>
</div>
    <div class = "signupbuttons">
        <a href= "https://frontend-tau-seven.now.sh/auth-register" class="button"><button>Sign Up</button></a>
        <a href= "https://frontend-tau-seven.now.sh/auth-login" class= "button"><button>Log In</button></a>
    </div>

<header>
    <h2>We take care of you!</h2>
    <h3>No more stress while traveling with kids! Sign up now!</h3>
    <img src= "Images/flying2.jpg" alt= "a picture of an airplane wing">
</header>


CSS and Less for my Project:

my imports for Less:

@import "variables.less";
@import "mixins.less";
@import "reset.less";
@import "global.less";
@import "navigation.less";
@import "home-page.less";
@import "about.less";


Service section for my Home-page:

.services {
    display: flex;
    width: 100%;
    justify-content: space-between;

    @media @phone{
        flex-direction: column;
    }
    
    .checkin{
        width: 30%;

        @media @phone{
            width: 100%;
        }
        img {
            width: 100%;
            height: 25vh;
            border-radius: 5px;

            @media @phone{
                height: 40vh;
            }
        }
    }
    .gate {
        width: 30%;
        @media @phone{
            width: 100%;
        }
        img{
           width: 100%;
           height: 25vh;
           border-radius: 5px;

           @media @phone{
               height: 40vh;
           }
        }
    }
    .luggage{
        width: 30%;
        @media @phone{
            width: 100%;
        }
        img{
           width: 100%;
           height: 25vh;
           border-radius: 5px;

           @media @phone{
            height: 40vh;
        }
        }
    }
}

my mixins: 

.aboutpeople () {
        display: flex;
        width: 40%;
        flex-direction: column;
        margin: 20px auto;

        @media @phone {
            width: 90%;
            margin-top: 1%;
        }
}

.picture(){
    border-radius: 5px;
    height: 45vh;
}


## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/buildweek-kidsFly-pg/UI/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/buildweek-kidsFly-pg/UI/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
