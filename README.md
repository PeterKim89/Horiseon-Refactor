# Horiseon-Webpage-Refactoring-Practice
![Horiseon](https://img.shields.io/badge/website-000000?style=for-the-badge&logo=About.me&logoColor=white)

## Introduction
This project was created to gain an insight at looking at another person's pre-existing code.
As developers, it is not only important to be able to write our own code, but read others' and give feedback. 
Instead of giving feedback, I refactored their webpage HTML and CSS to reduce redundancy and increase clarity.

## Build Process
- Gain a clear understanding of acceptance criteria
- Review pre-existing HTML and CSS
- Begin by creating semantics for easily identifiable elements E.g. Header, Footer, main, title
- Proceed to change the nested divs to more specific elements E.g. figures, articles, nav
- As changes were made to the HTML, the webpage was referenced to check for any changes
- If anything did change, the CSS was checked for any corresponding elements that may be responsible, and vice versa
- Any redundant CSS selectors were consolidated
- Comments were added throughout both HTML and CSS files

## Usage
[Deployment](https://peterkim89.github.io/Horiseon-Webpage-Refactoring-Practice/)

After following the url, the webpage should look like the following image.
The links in the navigation cluster should redirect the page to their respective areas.

![Webpage Template](/assets/images/01-html-css-git-homework-demo.png)

## Code Snippet
An example of consolidating the various benefit-* h3 classes into a single class.
```
.benefits section h3 {
    margin-bottom: 10px;
    text-align: center;
}

/* .benefit-lead h3 {
    margin-bottom: 10px;
    text-align: center;
}

.benefit-brand h3 {
    margin-bottom: 10px;
    text-align: center;
}

.benefit-cost h3 {
    margin-bottom: 10px;
    text-align: center;
} */
```

The large encapsulating div was changed into an aside, while the nested divs were changed into sections.
I also added alt text to each of the images.
Also because of the above CSS change, there was no longer a need for class tags to be used here.
```
<aside class="benefits">
    <section>
        <h3>Lead Generation</h3>
        <img src="./assets/images/lead-generation.png" alt="a gear funneling into a circle with a dollar sign"/>
        <p>
            Inbound strategies for lead generation require less work for your business, bringing customers directly to your website.
        </p>
    </section>
    <section>
        <h3>Brand Awareness</h3>
        <img src="./assets/images/brand-awareness.png" alt="a person with a shining lightbulb as their head"/>
        <p>
            Users find your business through paid and organic searches, increasing the search ranking and visibility for your business.
        </p>
    </section>
    <section>
        <h3>Cost Management</h3>
        <img src="./assets/images/cost-management.png" alt="a gear behind 3 circles with dollar signs on them" />
        <p>
            As the search ranking for your business increases, your advertising costs decrease, and you no longer need to advertise your page.
        </p>
    </section>
</aside>
```
## Contact
[GitHub](https://github.com/PeterKim89) <br>
[LinkedIn](www.linkedin.com/in/peter-kim89)    

## License
[MIT](https://choosealicense.com/licenses/mit/) <br>
Copyright (c) [2022] [Peter Kim]

