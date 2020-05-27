# Corvid - SPIs - Documentation Source Files
This repository includes all the documentation files for the Corvid - SPIs. The following documentation is visible through the [Corvid - SPIs Documentation](https://www.wix.com/corvid/new-reference/spis).

**Docs Server:** [Viewer Server Repository](https://github.com/wix-private/wix-public-corvid-spi-docs-viewer)

### Adding docs to the "API Reference" section in Wix Docs:

1. Follow our instructions in our [Docs Generation Guide](https://bo.wix.com/wix-docs/rnd/wix-docs-guides#how-to-generate-documentation).
2. Make sure your repo have a `documetation.yaml` file according to our [Documentation.yaml Guide](https://bo.wix.com/wix-docs/rnd/wix-docs-guides#documentation-yaml-guide.documentation.yaml-guide).

### Adding docs to the "Articles" section in Wix Docs:

 1. Write your guide in markdown syntax. You can either do it directly in Github, or using the following [Online Markdown Editor](https://stackedit.io/)
 2. Images - in case your markdown file is including images, you have two options to add them:
	 1. Full link to the image - in case the images are not stored in Github.
	 2. Relative link to the image - in case you want to use relative link to the image in this repo, you must locate the image in the `/media` folder.
 3. Upload your `.md` files to the `/guides` folder inside this repo. You can insert it to one of the existing folders in the `/guides` or create your own.
3. Go to the Wix Docs menu-config file [`/guides/guides.json`](./guides/guides.json) 
4. Add your file information in one of the existing categories. If you can't find a relevant category, you may add one. Add the following fields:
	1. `name` - the name you would like to show in the Wix Docs left menu.
	2. `url` - a relative link to your file.
	3. `isMdFile` - use `true` when the `url` is pointing for a markdown file.
	4. `isExternalLink` - use `true` when the `url` is pointing to an external link (will open in new tab)  
		for example:  
		  ```JSON  
		  {
		    "name": "Welcome",  
		    "url": "./welcome.md",  
		    "isMdFile": true  
		  },  
		  ```  

5. Commit & Push
6. Visit [Corvid - SPIs Documentation](https://www.wix.com/corvid/new-reference/spis) to find your article. 
	> **Be patient:** It takes ~10 minutes for the article to get online
	
	
### Organize the Wix Docs Menu - categories, order, names, etc

1. Go to the [Corvid - SPIs Menu Editor](https://www.wix.com/corvid/new-reference/spis/menu-editor).
2. Make you changes & export once you finish.
3. Send us the export config file to [#wix-docs](https://app.slack.com/client/T02T01M9Y/CC1U35ZRA) channel
