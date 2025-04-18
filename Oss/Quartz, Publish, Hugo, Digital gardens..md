---
tags:
  - discourse
  - garden
  - idea
  - journal
  - llm
  - selfhost
  - static
  - written
---
Ghost blog - profit 

write.as private anon? 
Part of https://musing.studio/start
Free, none Google. 
Commentory opinion personal


github pages 
Tech and how to

https://quaily.com/ 
Gnostic follow dao
Meaning
> All free until you start earning.
> ✅ Public Posts
> ✅ Send Newsletters
> ✅ Pay Posts
> ✅ Quaily AI
> ✅ Cooperative Edit
> ✅ Data Analayse
> ✅ Data Export
> ✅ Payment Methods
> ✅ Advance Editor
> 10% commission plus channel transaction fees will be charged after earning revenue
> 
Free
https://home.omg.lol/
- masterdon 20
- younger crowd





[dg-docs.ole.dev](https://dg-docs.ole.dev/getting-started/01-getting-started/)

# 01 Getting started

4 - 5 minutes

---

The initial setup takes a couple of minutes, but when you're done you'll have a digital garden in which you are in control of every part of it, and can customize it as you see fit. Which is what makes digital gardens so delightful.

1. Download and install the community plugin [Digital Garden](obsidian://show-plugin?id=digitalgarden) in Obsidian.

---

2. Next, you will need a GitHub account. If you don't have this, create one [here](https://github.com/signup).

---

1. You'll also need a Vercel account. You can sign up using your GitHub account [here](https://vercel.com/signup)

---

2. Open [this repo](https://github.com/oleeskild/digitalgarden), and click the blue "Deploy to Vercel" button.

  ![CleanShot 2023-01-22 at 23.38.57@2x.png](https://dg-docs.ole.dev/img/user/img/CleanShot%202023-01-22%20at%2023.38.57@2x.png)  
This should open Vercel and create a copy of this repository in your GitHub accont. Give it a fitting name like 'my-digital-garden'. Follow the steps in Vercel to publish your site to the internet.

---

3. Next you need to create an access token to your GitHub Account. This acts as a sort of password so that the plugin can add new notes to your GitHub repository on your behalf. Go to [this page](https://github.com/settings/tokens/new?scopes=repo) while logged in to GitHub. The correct settings should already be applied. (If you don't want to generate this every few months, choose the "No expiration" option.) Click the "Generate token" button, and copy the token you are presented with on the next page.

GitHub has recently launced a new beta feature, where you can target what repositories the token has access to. This is currently the most secure way to use the plugin. See [Fine grained access token](https://dg-docs.ole.dev/advanced/fine-grained-access-token/) for details on how to generate this.

---

4. Open Obsidian and the settings for "Digital Garden" and fill in your GitHub username, the name of the repo with your notes which you created in step 3, and lastly paste in your token.  
      ![CleanShot 2023-10-12 at 17.06.27@2x.png](https://dg-docs.ole.dev/img/user/CleanShot%202023-10-12%20at%2017.06.27@2x.png)
    
    ---
    
5. Now, let's publish your first note! Create a new note in Obsidian. Now add two new properties to the note.
    

Help! How do I add a property to a note  

Properties was added in Obsidian in [version 4.1](https://obsidian.md/changelog/2023-08-31-desktop-v1.4.5/)  
To add a property to a note, you have several options:

- Use the **Add file property** command.
- Use the **`Cmd/Ctrl+;`** hotkey.
- Choose **Add file property** from the **More actions** menu (three dots icon) or right-clicking the tab.
- Type `---` at the very beginning of a file.

- A checkbox named `dg-publish`
- A checkbox named `dg-home`  
    Toggle both checkboxes so that they are in the `checked` state.  
    It should look something like this:  
      ![CleanShot 2023-10-12 at 16.59.10@2x.png](https://dg-docs.ole.dev/img/user/CleanShot%202023-10-12%20at%2016.59.10@2x.png)

**This does two things:**

- The dg-home setting tells the plugin that this should be your home page or entry into your digital garden. (It only needs to be added to _one_ note, not every note you'll publish).
    
- The dg-publish setting tells the plugin that this note should be published to your digital garden. Notes without this setting will not be published. (In other terms: Every note you publish will need this property.)
    

---

6. Open your command pallete by pressing CTRL+P on Windows/Linux (CMD+P on Mac) and find the "Digital Garden: Publish Single Note" command. Press enter.

---

7. Go to your site's URL which you should find on [Vercel](https://vercel.com/dashboard). If nothing shows up yet, wait a minute and refresh. Your note should now appear.

---

Congratulations, you now have your own personal part of the internet in the form of a digital garden, for free 🎉.

You can now start adding links as you usually would in Obisidan, with double square brackets, to the note that you just published.

Remember to also publish the notes your are linking to as this will not happen automatically. This is by design. You are always in control of what notes you actually want to publish. If you did not publish a linked note, the link will simply lead to a site telling the user that this note does not exist.

If you want to unpublish a note, without deleting the note from your vault, simply uncheck or remove the dg-publish property in the note, open the [publication center](https://dg-docs.ole.dev/getting-started/02-commands/#open-publication-center) and click the "Delete notes from garden" button.

Now that you are up and running, you can take a look at the available [commands](https://dg-docs.ole.dev/getting-started/02-commands/) or the various available [note settings](https://dg-docs.ole.dev/getting-started/03-note-settings/). Or maybe you want to [change your theme](https://dg-docs.ole.dev/getting-started/04-appearance-settings/)?

[Next: Commands >](https://dg-docs.ole.dev/getting-started/02-commands/)
https://meta.discourse.org/t/install-discourse-in-production-with-the-official-supported-instructions/142537

---
https://meta.discourse.org/t/install-discourse-in-production-with-the-official-supported-instructions/142537

[https://meta.discourse.org/t/install-discourse-in-production-with-the-official-supported-instructions/142537]()

