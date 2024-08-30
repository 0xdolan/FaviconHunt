# **FaviconHunt** 🚀

Welcome to **FaviconHunt**, a repository dedicated to the collection and analysis of favicon hashes. This collection includes **38,299** unique favicon hashes gathered as part of OSINT activities in Bug Bounties.

## **Screenshot Gallery** 🖼️

Here’s a sneak peek of the collection:

![Favicon Hashes](assets/favicon_gallery.png)

## **Overview** 🔍

Favicon.ico hashes can be a powerful tool in the reconnaissance phase of cybersecurity efforts. By analyzing these hashes, you can identify new assets, IP addresses, and technologies that belong to a target organization. This repository serves as a centralized collection of these hashes, making it easier for you to utilize them in your own OSINT endeavors.

## **Features** ✨

- **Massive Collection:** Over **38,000** favicon hashes for comprehensive analysis.
- **Easy Integration:** Ready-to-use hashes for your OSINT tools and scripts.
- **Community Contribution:** Open to contributions and improvements from the community.

## **Favicon URLs List** 🌐

In the file **favicon_urls.txt**, you'll find a curated list of URLs that point to the favicon.ico files from which the hashes were generated. This list provides you with the source URLs to download and explore the favicons at your convenience.

### **How to Use the List** 🛠️

1. **Download the URLs List:**

   - The file `favicon_urls.txt` contains all the URLs pointing to the favicon.ico files.

2. **Download Favicons:**

   - You can use a tool like `wget` or `curl` to download the favicons from these URLs.
   - Example with `wget`:
     ```bash
     wget -i favicon_urls.txt -P ./favicons/
     ```
   - This command will download all the favicons into a directory named `favicons`.

3. **Analyze the Favicons:**
   - Once downloaded, you can view and analyze the favicons using your preferred tools.

## **Extracting Favicon Hashes** 🔍

To extract the favicon hashes from the provided list of URLs, you can use the following `sed` command. This command handles various file extensions and outputs only the hashes:

```bash
sed -E 's|.*/favicon_(-?[0-9]+)\.[^.]+|\1|' favicon_urls.txt
```

**Note:** This repository only provides the list of URLs; you are responsible for downloading the favicon.ico files and ensuring their legal use.

## **Usage** 💻

Clone the repository and use the hashes in your favorite OSINT tools to uncover hidden assets and technologies.

```bash
git clone https://github.com/yourusername/FaviconHunt.git
```

## **Contributing** 🤝

We welcome contributions from the community! Whether it's adding new hashes, improving the existing collection, or enhancing documentation, feel free to submit a pull request. Please make sure that your contributions adhere to the project's guidelines.

## **License** 📜

This project is licensed under the GNU General Public License (GPL). See the [LICENSE](LICENSE) file for details.
