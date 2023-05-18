# flask-blog-website

Little update...Instead of getting hold of blog posts from the npoint JSON bin, I grab the posts from the posts.db SQLite database that's included in the starting project.

I created a new POST route called /new-post in Flask server. It is rendering the make-post.html page when someone click on the "Create New Post" button.
Also I use the Flask CKEditor package to make the Blog Content (body) input in the WTForm into a full CKEditor.

When the user is done typing out entries to all the fields, the data in the form are saving as a BlogPost Object into the posts.db .
Once the post is saved, the user is redirecting to the home page and the new post is showing up if the saving process was successful.

At the end of the post, is an Edit Post button. When the user clicks on the "Edit Post" button at the bottom of any blog post it makes a GET request to this route.

In index.html was created an anchor tag that just shows a ✘ character next to each post. When someone click on it, it should delete the post from the database and redirect the user to the home page.

I've build a very simple blog with a number of blog posts. Where you can see the title and subsitle. And also you can click on More to see the blog post in detail, you go to a different page. 
![image](https://github.com/pradomska/flask-blog-website/assets/113101087/a4593b86-2964-4ec1-8725-4c3fe8568908)

And depending on which of these blog posts you've clicked on, you can see that I'm rendering basically the same layout, the same styling and the same structure, each time for each of these pages, you're getting some different content. Also I add a clickable title to come back to home page.
