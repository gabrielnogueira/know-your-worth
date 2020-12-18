[![Netlify Status](https://api.netlify.com/api/v1/badges/624765bd-73de-4e74-bb40-cf40b7cefc5e/deploy-status)](https://app.netlify.com/sites/know-your-worth/deploys)

### What is this

After watch a [video on youtube](https://www.youtube.com/watch?v=Ce_Y3hyvHdo) about software engineer compensations i went through a research about this subject to understand better what could be the pros and cons about share info about our salary.

After a few researh and reading good things about share our salary with people around us and our coworkers, i got noticed that some people motivated by a [Zac Sweer's tweet](https://twitter.com/ZacSweers/status/1228205724255154177) started share your salary info on that thread.

Like spoken on the video above, i saw a big problem sharing these info on social media: security

### Why this

If you area a influent person and your twitter is most for business about your profession probably this reason don't apply to you. But if you are a normal person normally you will have a lot of closer people following you on your social media, like friends, colegues, neighbors, etc.

On a developed country with low criminal rates tell your salary to everybody could not be a problem to you. But for the most of people that live a different life in a poor country with high criminal rates, your neightbor know about your compensations could bring to you serious problem on the future. 

So i build these simple site - following Zac advice - to share with our community our salary and according to these info we can try to know how much we worth on the place that we are and eradicate a big problem in our area:

> *"Pay inequality is a big problem in tech, especially for underrepresented groups like women and minorities. The best way you can help is by sharing yours."*<br>
> — <cite>Zac Sweers[^1]</cite>

[^1]: The above quote is excerpted from Zac Sweers's [tweet](https://twitter.com/ZacSweers/status/1228205724255154177) on February 14, 2020.

### Legend

🎓 - Degree  
⏳  - Experience  
👔 - Position  
🌎 - Location  
💸 - Salary  
📑 - Job type 
  
  
  
**Salary / Cost of Living index:**  

  
```go
index := totalSalary * .65 / 12 / locationIndex

if(index < 2){
    // Low - red
}else if (index < 5){
    // Normal - orange
}else if (index < 12){
    // High - yellow
}else{
    // Franking High - green
}
```


### Contribute

To contribute, you just have to create a PR to the branch new-posts on this project including a ***@mynickname.md*** file inside /posts folder with your data.

Follow this template:

```yaml
---
title: "" #@mytwitter @mygithub...
date: 2020-12-16T23:38:14-03:00 #todays data
draft: false

name: "" # My Name
social: "" #@mytwitter @mygithub...
picture: "" #public avatar url
socialUrl: ""
degrees: "" #self taught, computer science, MBA...
experiences: "" #12 years
positions: "" #senior software engineer
locations: [] #[city, country]
salaries: "" #40k base | 100k bonus
salaryTotal: 0 #240000.00 all annual compensation sum
locationIndex: 0 #450.35 a single person estimated monthly costs without rent in numbeo.com to your location
types: "" #permanent, contractor 
---

<!-- how do i get here -->
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
```

If you are not familiar with github, To do that, just:

    - Fork the project
    - Make a new branch
    - Include your .md file
    - Click the Compare & pull request button
    - Click Create pull request to open a new pull request

More info at: https://opensource.com/article/19/7/create-pull-request-github
