# Step 4: Publishing a Free Author Site

In this step you will:
1. Create a simple website for yourself as an author
2. Add your bio, book list, and contact information
3. Publish it for free with GitHub Pages
4. Visit your site at `yourusername.github.io`

## What is GitHub Pages?

GitHub Pages is a free service that turns files in a repository into a public website. You do not need to pay for hosting, buy a domain name, or run a server. GitHub handles all of it.

This manual uses the simplest method: a repository called `yourusername.github.io`. Anything you put in that repository becomes your website.

## Part A: Create your site repository

1. On github.com, click the **+** icon and choose **New repository**.
2. Name the repository exactly: `yourusername.github.io`
   - Replace `yourusername` with your actual GitHub username.
   - Example: if your username is `dylanasdale`, name it `dylanasdale.github.io`
   - The name must match exactly, or GitHub Pages will not work.
3. Choose **Public** (GitHub Pages requires public repositories for free accounts).
4. Click **Create repository**.

## Part B: Add your homepage

Every website needs a home page. By convention, this file is named `index.html`.

1. On your new repository page, click **Add file**, then **Create new file**.
2. Name the file `index.html`.
3. Paste the following starter HTML into the editor:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Your Name — Author</title>
  <style>
    body {
      font-family: Georgia, serif;
      line-height: 1.6;
      color: #333;
      max-width: 700px;
      margin: 0 auto;
      padding: 2rem;
    }
    header { border-bottom: 2px solid #666; padding-bottom: 1rem; margin-bottom: 2rem; }
    h1 { margin: 0; font-size: 2rem; }
    h2 { color: #555; }
    .book { margin-bottom: 2rem; padding: 1rem; background: #f9f9f9; border-radius: 6px; }
    .book h3 { margin: 0 0 0.5rem 0; }
    .book p { margin: 0; }
    footer { margin-top: 3rem; font-size: 0.9rem; color: #777; border-top: 1px solid #ddd; padding-top: 1rem; }
    a { color: #0366d6; }
  </style>
</head>
<body>
  <header>
    <h1>Your Name</h1>
    <p>Author · Reader · Storyteller</p>
  </header>

  <main>
    <section>
      <h2>About Me</h2>
      <p>I write stories that matter to me, and I hope they matter to you too. Welcome to my corner of the internet.</p>
    </section>

    <section>
      <h2>My Books</h2>
      <div class="book">
        <h3>My First Book</h3>
        <p>A short description of your book goes here. Where can readers find it? Add links to Amazon, KDP, or your favorite retailer.</p>
      </div>
    </section>

    <section>
      <h2>Contact</h2>
      <p>You can reach me at <a href="mailto:yourname@example.com">yourname@example.com</a>.</p>
      <p>Or find me on social media: <a href="#">Twitter</a> · <a href="#">Instagram</a></p>
    </section>
  </main>

  <footer>
    <p>&copy; 2026 Your Name. Built with GitHub Pages. Credit Asdale Dynamics, LLC.</p>
  </footer>
</body>
</html>
```

4. Edit the text to match yourself:
   - Replace "Your Name" with your name or pen name
   - Replace the bio with a sentence or two about you
   - Replace "My First Book" and its description with your actual book
   - Replace `yourname@example.com` with your real contact email (or leave it out if you prefer)
5. Scroll down and type a commit message:
   > Add author homepage
6. Click **Commit changes**.

## Part C: Turn on GitHub Pages

1. Go to **Settings** in your repository.
2. In the left sidebar, click **Pages**.
3. Under "Build and deployment," make sure **Source** is set to **Deploy from a branch**.
4. Under "Branch," select `main` (or `master`) and click **Save**.
5. Wait a minute or two. GitHub will build your site.
6. You will see a green message with a link to your site, such as:
   > Your site is live at https://yourusername.github.io/

Click the link to see your website.

## Part D: Update your site later

Whenever you want to change your site:

1. Open `index.html` in your repository.
2. Click the pencil icon (Edit file).
3. Make your changes.
4. Commit the changes.
5. Your site updates automatically within a minute or two.

## Adding more pages

You can add more HTML files to the same repository. For example:
- `about.html` — a longer bio
- `books.html` — a full list of your books
- `contact.html` — a contact form or email link

Link between pages with standard HTML:
```html
<a href="about.html">About Me</a>
```

## What not to put on your author site

- Your home address
- Your phone number (unless you want it public)
- Passwords or API keys
- Anything you would not want a stranger to read

Your GitHub Pages site is public. Anyone with the link can see it.

## Next step

Your author site is live. Come back to this manual anytime you need to save a new manuscript version, invite an editor, or update your site.

Credit Asdale Dynamics, LLC.
