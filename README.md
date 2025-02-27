# LPLI1994
A brief summary of [Let's Party Like It's 1994: Reimagining How to Find Stuff Online, By Martin Hamilton](https://m.youtube.com/watch?v=iJ1PXzeQHVA) EMF2024.

## [Martin's abstract from EMF](https://www.emfcamp.org/schedule/2024/13-lets-party-like-its-1994)

Internet search results were a toxic hellstew of ads, SEO spam, content farms and misinformation/disinformation even before the arrival of Large Language Models like ChatGPT in 2023. In 2024 nearly half the world’s population votes in elections that will have consequential impacts for key issues like climate change and civil rights, and it’s more important than ever before that search results can be relied upon.

This talk will highlight a few ways to put search back in the service of the searcher rather than a handful of global megacorps. We’ll time-travel 30 years to the Internet’s Cambrian Explosion period, before Lycos, AltaVista and BackRub/PageRank, and look how technologies like Really Simple Syndication (RSS) and open source self-hosted meta-search engines like SearXNG can help. And then, demo gods permitting, I’ll show you how this can all come together to put a search engine in every pocket

---

# Summary

## Why consider alternatives?

The mainstream search landscape has evolved dramatically from the "pure search" days of early Google to today's experience filled with:

- Excessive sponsored content and ads
- Self-promotion of proprietary services
- Privacy concerns and tracking
- Content filtering and potential censorship
- AI-generated results with potential inaccuracies

## Notable alternative search engines

### Privacy-focused search engines

<div style="overflow-x: auto;">

| Search engine | URL | Key features | Business model |
|---------------|-----|--------------|---------------|
| **DuckDuckGo** | [https://duckduckgo.com](https://duckduckgo.com) | No personal tracking, private browsing | Ads based on search keywords only |
| **Startpage** | [https://startpage.com](https://startpage.com) | Google results without tracking, Anonymous View | Non-personalized ads |
| **Brave Search** | [https://search.brave.com](https://search.brave.com) | Independent index, no tracking | Freemium (basic search free, premium features paid) |
| **Qwant** | [https://www.qwant.com](https://www.qwant.com) | European privacy-focused engine | Ads based on keywords only |
| **SearX** | [https://searx.space](https://searx.space) (instances list) | Self-hostable metasearch engine | Open-source, no ads |

</div>

### Subscription-based search

<div style="overflow-x: auto;">
   
| Search engine | URL | Key features | Business model |
|---------------|-----|--------------|---------------|
| **Kagi** | [https://kagi.com](https://kagi.com) | Ad-free, customizable, AI features | $10/month subscription |
| **Neeva** | [https://neeva.com](https://neeva.com) | Ad-free, includes personal accounts integration | Subscription-based (recently acquired by Snowflake) |

</div>

### Independent index engines

<div style="overflow-x: auto;">
   
| Search engine | URL | Key features | Business model |
|---------------|-----|--------------|---------------|
| **Mojeek** | [https://www.mojeek.com](https://www.mojeek.com) | UK-based independent crawler and index | Ads (with privacy focus) |
| **Yep** | [https://yep.com](https://yep.com) | Independent index from Ahrefs | Ads with 90% revenue sharing to content creators |
| **Noir** | [https://noir.essearch.eu](https://noir.essearch.eu) | EU initiative for European search engine | Government/EU funded |

</div>

### Specialized search engines

<div style="overflow-x: auto;">
   
| Search engine | URL | specialization | notes |
|---------------|-----|--------------|---------------|
| **Ecosia** | [https://www.ecosia.org](https://www.ecosia.org) | Eco-friendly | Uses profits to plant trees |
| **Presearch** | [https://presearch.org](https://presearch.org) | Decentralized | Uses blockchain and node operators |
| **You.com** | [https://you.com](https://you.com) | AI-integrated | Chat interface with web search |
| **Perplexity** | [https://www.perplexity.ai](https://www.perplexity.ai) | AI research assistant | Combines search with AI synthesis |

</div>

## Setting up UDM-14 (Google's "clean search" mode)

UDM-14 is a parameter discovered in Google Search URLs that removes AI overviews and many promotional elements, providing a cleaner search experience reminiscent of earlier Google.

### Method 1: Using UDM-14.com

The simplest approach is to use the UDM-14.com service:

1. Visit [https://udm14.com/](https://udm14.com/)
2. Follow the instructions to add it as your default search engine

### Method 2: Manual browser configuration

#### For Chrome:
1. Go to Settings > Search engine > Manage search engines
2. Click "Add"
3. Enter:
   - Search engine: "Google Clean"
   - Shortcut: "g" (or your preference)
   - URL: `https://www.google.com/search?q=%s&udm=14`
4. Click "Add"
5. Find "Google Clean" in your list and click "Make default"

#### For Firefox:
1. Right-click the address bar and select "Add a Keyword for this Search"
2. Visit Google.com
3. Right-click the search box and select "Add a Keyword for this Search"
4. Name it "Google Clean" with keyword "g"
5. Edit the URL to add `&udm=14` before saving
6. Alternatively, install an add-on like "Add custom search engine"

#### For Safari:
1. Create a bookmark with this URL: `https://www.google.com/search?q=%s&udm=14`
2. Edit the bookmark to add a keyword like "g"

### Method 3: Browser extensions

Several browser extensions automate the addition of UDM-14:

- "Google Sans AI" ([https://chromewebstore.google.com/detail/google-sans-ai/jooddajpanbdklojchgaaniamjlcknmn](https://chromewebstore.google.com/detail/google-sans-ai/jooddajpanbdklojchgaaniamjlcknmn)) for Chrome
- "Unprompted" ([https://github.com/chiefonboarding/Unprompted](https://github.com/chiefonboarding/Unprompted)) for multiple browsers
- "uBlacklist" ([https://github.com/iorate/uBlacklist](https://github.com/iorate/uBlacklist)) can be configured to clean up search results

## Building your own search solution

For the technically inclined, consider:

### Self-hosted search options
- **SearXNG**: [https://github.com/searxng/searxng](https://github.com/searxng/searxng) - A privacy-respecting metasearch engine you can self-host
- **Whoogle**: [https://github.com/benbusby/whoogle-search](https://github.com/benbusby/whoogle-search) - A self-hosted, privacy-focused Google search proxy
- **YaCy**: [https://yacy.net](https://yacy.net) - Decentralized, peer-to-peer search engine network

## Advanced customization

### Using search aggregators
Tools like LibreX ([https://github.com/hnhx/librex](https://github.com/hnhx/librex)) and SearXNG let you combine results from multiple search engines.

### Creating custom search experiences
- Use RSS feeds and site maps to build targeted search
- Implement shared blocklists for filtering unwanted content
- Deploy search containers for portable search solutions

## Final thoughts

By being more "goat" than "sheep" (to use Martin's metaphor), you can reclaim control over your search experience, protect your privacy, and potentially access more diverse, less manipulated search results.

Remember that the perfect search engine is the one that best meets your specific needs and values.

---

*This guide was produced with assistance from Claude 3.7 Sonnet, February 2025, based on YouTube's transcript of Martin Hamilton's talk "Let's Party Like It's 1994: Reimagining How to Find Stuff Online".*

---

**All credit and thanks to [Martin Hamilton](https://martinh.net)**
