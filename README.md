# Blog Network Link Mapper

A free, single-page tool for people who run more than one Blogger blog. Enter your blog addresses, and it maps how your blogs link to each other.

**Try it:** https://zayzaria.github.io/Blog-Network-Link-Mapper/

## What it shows

- **Who links to whom:** a grid of which blog links to which, counted by posts and pages
- **One-way links:** blog A links to blog B, but B never links back
- **Pages nothing links to:** posts and pages that no other post or page in your network points to (search engines find these slowly)
- **Old `http://` links** between your blogs that should be `https://`
- **Your profiles on each blog:** add your YouTube, X, LinkedIn, Facebook (or any other) profile links, and see which blogs link to each one and which are missing them
- **Every link between your blogs**, listed with the page it's on
- A **Copy report** button for a plain-text summary

## How it works

It reads each blog's public Blogger feed (`/feeds/posts/default` and `/feeds/pages/default`) straight from your browser. Nothing is sent to a server, there's no sign-in, and nothing is stored.

## Requirements and limits

- Works with **Blogger** blogs, on blogspot.com or a custom domain.
- The blog feed must be on: **Settings → Site feed → Allow blog feed** set to **Full**. If it's set to **Short**, only the start of each post is read, and the tool warns you.
- It counts links **inside posts and pages**. Header menus, sidebar gadgets and footers are part of the theme and aren't in the feed, so they aren't counted.

## Use it on your own Blogger blog

1. Open `index.html` and copy everything from the `<style>` line down to the closing `</script>`.
2. In Blogger, create a new **Page**, switch to **HTML view**, and paste it in.
3. Change the example blogs and profiles at the top of the script (`EXAMPLE_BLOGS` and `EXAMPLE_PROFILES`) to your own, or leave them blank.

## Host it on GitHub Pages

1. Fork or copy this repository.
2. Go to **Settings → Pages**, set **Source** to **Deploy from a branch**, choose `main` and `/ (root)`, and save.
3. After a minute, it's live at `https://YOUR-USERNAME.github.io/blog-link-mapper/`.

## About the maker

Made by Tiza, who has been building websites since 1996.

**My blogs**
- [Queen of France](https://www.queen-of-france.com/): AI prompt generator tools
- [Magi Chef](https://magi-chef.blogspot.com/): recipes and the grocery-to-dinner Recipe Builder
- [Magi Gamer](https://magi-gamer.blogspot.com/): free arcade and puzzle games
- [DNS Tools](https://dns-tools.blogspot.com/): DNS, WHOIS and network tools
- [Social Link Banners](https://social-link-banners.blogspot.com/): social and AI link banners
- [One Page Wonders](https://one-page-wonders.blogspot.com/): one-page calculators and tools
- [Tutu Ballerina](https://tutu-ballerina.blogspot.com/): ballet
- [Ballerina Pointes](https://ballerina-pointe-shoes.blogspot.com/): pointe shoes

**Find me**
- [YouTube](https://www.youtube.com/user/zayvra) · [zayvra.com](https://zayvra.com)
- [X](https://x.com/zayvra)
- [LinkedIn](https://www.linkedin.com/in/therese-vaux/)
- [Facebook](https://www.facebook.com/theresevaux.fontaine.9)

## License

MIT. Free to use, change and share. See [LICENSE](LICENSE).
