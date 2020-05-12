# Vercel-now-namecheap-setup
How to set up Namecheap Private Email records for domains with third-party DNS with Vercel via `CLI now` commands 

## Objective

I created this documintation so that you will have a step by step guide on setting up your DNS records from Namecheap with Vercel now. After reading through this documintation, you should be able to have your DNS configured with Vercel now successfully. 

### Technologies

- Vercel CLI
- Namecheap

### Instructions

Make sure to replace `yourdomain.com` with your domain name. If you need help with the command type `now dns --help` in your CLI

`now dns add yourdomain.com @ TXT v=spf1include:spf.privateemail.com~all`

`now dns add yourdomain.com @ MX mx1.privateemail.com 10`

`now dns add yourdomain.com @ MX mx2.privateemail.com 10` 
 
 ### Docs 
 - [list of the essential records](https://www.namecheap.com/support/knowledgebase/article.aspx/1340/2176/namecheap-private-email-records-for-domains-with-thirdparty-dns)
 - [install Vercel](https://vercel.com/download)
 
 ## Conclusion
 
In conclusion, you should now be able to login to your Vercel Dashboard, and under "Recently Active" you should see a message: "You added a DNS record for yourdomain.com" for MX and TXT. 

Inspired by [zeit now g-suite-setup](https://gist.github.com/jaydenseric/cf7e548d3ce035da05fae5782878b80f)





