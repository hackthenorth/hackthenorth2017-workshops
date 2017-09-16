# Web Dev 2 (Frontend)

## Getting Started with VueJS
To start a project with VueJS, use Vue CLI: https://vuejs.org/v2/guide/installation.html#CLI
Once you have a Vue project running, use `{{ var }}` to print variables in your HTML.
Vue objects have two special properties: *data* and *methods*. These can be accessed from the HTML.
To repeat an element multiple times in a list, use `v-for="item in var"`.

Looking for a super quick way to get started? You can include Vue like any other script and still get lots of features: https://vuejs.org/v2/guide/installation.html#Direct-lt-script-gt-Include

## The Reddit API
To display data from an API, it’s often easiest to retrieve the data in JSON format.
To get the top 25 Reddit posts, send a GET request to https://reddit.com/top.json
To search the top Reddit posts, send a GET request to https://reddit.com/search.json?q=searchText&sort=top
All responses have a `data.children` property. This is an array with the post data.
Each post in that array has a `data` property with properties like `title`, `subreddit`, and `score`.

Want to learn more about the Reddit API? All docs are available here: https://www.reddit.com/dev/api/
Take a look at the full responses returned by the Reddit API using a JSON viewer extension like this one: https://chrome.google.com/webstore/detail/jsonview/chklaanhfefbnpoihckbnefhakgolnmc?hl=en

## Plugging the Reddit API into Vue
The Fetch API can be used to send GET requests from Javascript.
Use the `response.json()` function to transform the response into JSON.
When a Vue component loads, the `created()` function is called. Use this to fetch any data you need when the page first loads.

The `created()` function isn’t the only special function in Vue. There are several others, and they’re collectively known as Lifecycle Hooks: https://vuejs.org/v2/guide/instance.html#Instance-Lifecycle-Hooks

## Searching
Use `v-model` to tie the value of an input to a variable.
To call `myFunction()` when a button is clicked, use `v-on:click=”myFunction”1.
To update your HTML, simply change the value of a variable to see it updated live.

You don’t need to trigger all your functions with clicks. You can also trigger functions on form submit or on keypress: https://vuejs.org/v2/guide/events.html

You can find out lots more about Vue with their official guide:
https://vuejs.org/v2/guide/
