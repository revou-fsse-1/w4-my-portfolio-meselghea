# A Step-by-Step Guide: </br> Deploying Website & Custom Domain

Website: [Mesel Ghea Personal Site](https://meselghea.site/)

## Deploying Website on netlify

### Step 1: Login to your [Netlify](https://app.netlify.com/)

![netlify login](photo/Netlifylp.png)

#### Step 2: Click menu " site "

![netlify menu site](photo/sitemenunetlify.png)

### Step 3: Click " Add New Site " > " Import an existing project "

![import new site](photo/importnewsitenetlify.png)

### Step 4: Connect to Git provider & pick a your respository

![import new site](photo/importnewsitenetlify.png)

### Step 6: Skip the basic build settings & click " deploy site "

If you’re not using a static site generator or build you skip

![deploy site](photo/deploysitenetlify.png)

## Connect to domain and DNS

### Step 1: Purchase a domain from a hosting provider

Hosting Provider: [Niagahoster](https://www.niagahoster.co.id/), [Hostinger](https://www.hostinger.co.id/), [Domainesia](https://www.domainesia.com/)

![buy domain](photo/buydomainniagahoster.png)

### Step 2: Setting DNS with Cloudflare

- Login to your [cloudframe](https://dash.cloudflare.com/login)
  ![login cloudflare](photo/logincloudflare.png)
- Click Websites > add a site > input your custom domain
  ![input custom domain](photo/inputcustomdomain.png)
- Copy cloudflare nameservers to provider hosting
  ![cloudflare nameservers](photo/cloudflarenameservers.png)
  If you use Niagahoster, go to "Kelola Layanan" > Overview Domain > "Ubah Nameserver"
  ![kelola layanan](photo/kelolalayananniagahoster.png)
  ![overview](photo/ubahnameserver.png)
  ![nameserver](photo/namesarver.png)
- Setting CNAME on Cloudflare,
  click DNS > Records > Add Record > change type A to CNNAME > copy custom domain at column name > copy Netfliy site to content
  ![input custom domain](photo/settingcname.png)

### Step 3: Add Custom Domain to Netlify

- Open Netlify, click domain Setting
  ![domain setting](photo/domainsetting.png)
- Scroll down > click Add a Domain > copy your custom domain
  ![add domain](photo/addomain.png)
