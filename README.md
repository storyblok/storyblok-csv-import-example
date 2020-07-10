<center>
  <h1>Storyblok CSV Import Example</h1>
</center>

Simple example on how to read a CSV and push each line into Storyblok.

## How to use

### Install the dependencies of the project

```sh
npm install 
```

### Configure the project

In the **./index.js** 

```js
const Storyblok = new StoryblokClient({
  oauthToken: 'Your_Personal_access_tokens' // Add your Personal access tokens here
  /* To obtain this access token, you need to be logged in to the storyblok and got My account> Personal access tokens, and copy or gene a new token
  */
})

const config = {
  spaceId: 'Your_Space_Id', // To get the spaceid enter the desired space, go to the settings>General menu and copy the space_id
  parentFolder: 'Your_Folder_Number' // navigate into your folder and copy the id from the URL at app.storyblok.com <- last one 
}
```

### Run the project

```sh
node index.js
```

---

<p align="center">
  <h5 align="center">Powered by <a href="https://www.storyblok.com/" title="link to the Storyblok website">Storyblok</a></h5>
</p>
