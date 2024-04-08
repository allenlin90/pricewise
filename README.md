# Features
- Users can check products on `amazon` to track on price of a product and send email notification with cron job on daily basis. 
- Cron job is triggered using `cron-job.org`. 

# Tech stack
- [Bright data](https://brightdata.com/) - A proxy mocking real users using browsers browsing web page/apps.
- [cheerio](https://www.npmjs.com/package/cheerio) - A text parser using jQuery like syntax. 
- [React responsive carousel](https://www.npmjs.com/package/react-responsive-carousel) - A React based responsive carousel component. 
- [Headless UI React](https://www.npmjs.com/package/@headlessui/react) - Completely unstyled, fully accessible UI components working with Tailwind CSS.
- [nodemailer](https://www.npmjs.com/package/nodemailer) - send emails from Node.js
- [cron-job.org](https://console.cron-job.org/) - A cron job service provider to test hitting APIs. 

## BrightData
### Web Unlocker
1. This is the proxy we used from BrightData to scrape the other websites
2. We only give a `solution` name without geo location targeting, premium domains, async requests, nor advanced options for custom headers and cookies. 
3. We will refer to the `host` of the proxy scraper such as `brd.superproxy.io:22225`, `username`, and `password`.
4. Note that we keep `username` and `password` in environment variables. 

# Todo
## Product details
- Like on the product
- Reviews count on the product
- Percentage of buyers recommendation
- Average price of a product
- Highest price of a product
- Lowest price of a product

# Known issue on Vercel
- `lib\nodemailer\index.ts` may have timeout (max 10 seconds for free `hobby` plan) on vercel serverless/edge function.
