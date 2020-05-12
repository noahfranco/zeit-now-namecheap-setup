# zeit-now-namecheap-setup
How to set up Namecheap Private Email records for domains with third-party DNS with Zeit via `CLI now` commands 

## Objective

I created this documintation so that you will have a step by step guide on setting up your DNS records from Namecheap with Zeit now. After reading through this documintation, you should be able to have your DNS configured with Zeit now successfully. 

### Technologies

- Zeit now
- Vercel
- Namecheap

### Instructions

Make sure to replace `yourdomain.com` with your domain name. If you need help with the command type `now dns --help` in your CLI

`now dns add yourdomain.com @ TXT v=spf1include:spf.privateemail.com~all`

`now dns add yourdomain.com @ MX mx1.privateemail.com 10`

`now dns add yourdomain.com @ MX mx2.privateemail.com 10` 
 
 ### Docs 
 - [list of the essential records](https://www.namecheap.com/support/knowledgebase/article.aspx/1340/2176/namecheap-private-email-records-for-domains-with-thirdparty-dns)





