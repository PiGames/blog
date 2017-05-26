---
layout: post
title:  "Welcome to Jekyll!"
date:   2017-05-26 18:38:32 +0200
author: bibixx
categories: jekyll update
---
You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

```javascript
import { foo } from '../bar';
class Cat {
  constructor(name) {
    this.name = name;
  }

  speak() {
    console.log(this.name + ' makes a noise.');
    foo();
  }
}

class Lion extends Cat {
  speak() {
    super.speak();
    console.log(this.name + ' roars.');
  }
}

var l = new Lion('Fuzzy');
l.speak();
// Fuzzy makes a noise.
// Fuzzy roars.
```

```sass
code[class*="language-"], pre[class*="language-"]
  color: black
  background: none
  text-shadow: 0 1px white
  font-family: Consolas, Monaco, 'Andale Mono', 'Ubuntu Mono', monospace
  text-align: left
  white-space: pre
  word-spacing: normal
  word-break: normal
  word-wrap: normal
  line-height: 1.5
  -moz-tab-size: 4
  -o-tab-size: 4
  tab-size: 4
  -webkit-hyphens: none
  -moz-hyphens: none
  -ms-hyphens: none
  hyphens: none
```

```csharp
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Arrow : MonoBehaviour
{
    public static Arrow instance;

    //Singleton
    public static Arrow getInstance()
    {
        if (instance == null)
        {
            return null;
        }
        else return instance;
    }

    // Use this for initialization
    void Start()
    {
        //Code checking if exist only one instance of class
        if (instance != null) Destroy(this);
        else instance = this;
        //
    }

    // Update is called once per frame
    void Update()
    {
        rotationUpdate();
    }

    void rotationUpdate()
    {
        if(Rocket.getInstance() != null)
        {
            var direction = GameObject.FindGameObjectWithTag("Airstrip").GetComponent<Transform>().position - Rocket.getInstance().GetComponent<Transform>().position;
            var angle = Mathf.Atan2(direction.y, direction.x) * Mathf.Rad2Deg;
            transform.rotation = Quaternion.AngleAxis(angle, Vector3.forward);
        }

    }
}
```

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
