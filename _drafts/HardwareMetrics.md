---
layout: post
title: Hardware Part 2
---
As any founder of a hardware company knows, many venture capitalists are reluctant (or even unwilling) to invest in such businesses. There is a widespread perception that this attitude stems from the inherently lower gross margins of such businesses. This is certainly part of the story, but it's far from the whole picture. In truth, it all comes back to "scalability." In this post, I want to lay out a set of important questions that are uniquely relevant to hardware companies.

Venture investors are seeking a very specific company profile in order to deliver the returns that their investors require. In general, VCs want to invest in companies that could achieve a one billion dollar valuation in five to ten years if everything breaks just right. This requirement is rooted in the risk/return profile of the asset class, a full discussion of which is outside the scope of this post. For a fuller discussion of the topic, check out [this post](https://www.sethlevine.com/archives/2014/08/venture-outcomes-are-even-more-skewed-than-you-think.html) by Seth Levine from Foundry Group. 

Hyper-growth isn't the only characteristic VCs are looking for, however. Investors also want to understand the capital required to achieve such growth, and most are wary of businesses that will consume vast amounts of capital to get to scale. This is doubly true for early stage investors with smaller funds who will be unable to participate in gigantic late-stage funding rounds and who will experience significant dilution of their ownership.

The first question to ask yourself is "What does a billion-dollar company look like?" This will vary significantly by industry and with business model. A quick and dirty method for estimating this is the revenue multiple which you can look up for public companies similar to yours. With this in hand, simply divide $1B by the revenue multiple to get the required revenues for your business. SaaS companies, for example, can see revenue multiples of 8-10x which implies ~$100M in revenue for a billion dollar valuation. The GAP, on the other hand, has a revenue multiple of 0.6, implying a much higher revenue threshold for apparel retailers to see an equivalent valuation. Whatever the number is for your business, you can use it to back into the number of unit sales you'll need to hit for a "venture scale" outcome.

With the goal posts set, the question then becomes, "what will it take for us to get there in five to ten years?" There are two key components to answering this question: capital requirements and supply chain complexity.

## Working Capital
Hardware businesses often require large amounts of capital for two purposes that their software brethren don't: equipment (ie. cap ex) and inventory (ie. working capital). Both operators and investors generally try to minimize the equity capital required for these purposes. This can be achieved both through savvy business practices and by using debt capital rather than equity once you have achieved sufficient scale.

One of the most significant metrics for understanding the capital needs of the business is the Cash Conversion Cycle (CCC), which is the number of days it takes the company to convert investments in inventory into revenue. The longer the CCC, the more working capital you will require to operate your business.

~~~
CCC = DSI + DSO - DPO. 
DSI = Days sales in inventory
DSO = Days sales outstanding
DPO = Days payable outstanding
~~~

Simply put this relationship says that a company can shorten its cash conversion cycle by holding less inventory, paying its suppliers more slowly, and collecting from customers more quickly. MBA math: it's not rocket science. Let's walk through each of these items.

### Days Sales in Inventory

DSI = Average Inventory Balance/COGS. This measures how long it takes you to cycle through  We want a low DSI value, which we can achieve by reducing our inventory levels. Assuming an optimal inventory policy, the average inventory balance is directly proportional to demand, lead times from suppliers, and desired service level. Each of these variables are the focus of questions below. 

### Days Sales Outstanding

DSO = Average Accounts Payable/Sales. Simply put, this measures how long it takes you to collect from your customers once they buy a product. Obviously lower is better here. If you are able to get paid up front (or even better, in advance!), you can drive your CCC down significantly.

### Days Payable Outstanding

DPO = Average Accounts Payable/COGS. This is a measurement of how long it takes you to pay your suppliers. You can directly increase this metric (and thereby reduce CCC) by negotiating more favorable payment terms with suppliers. Many vendors will require prepayment or COD (cash on delivery) for young companies, but many will be willing to offer more favorable terms (ie net-20 or net-30) once a track record has been established. 

### Key Questions:

* Are you manufacturing in house or outsourcing? 
    * If in-house, there had better be a very good reason _and_ a plan to keep the required equity investments in line with business milestones/de-risking. Alternative forms of financing, including venture debt, may be appropriate to fund CapEx.
    * If outsourcing, then you need to understand both minimum order quantities (MOQ) and manufacturer's margin. MOQ is much more important in the short term; margin is more important long-term.
* Assuming you outsource manufacturing, can your provider drop-ship for you?
    * If yes, what will they charge you for the convenience? 
    * Will they be producing just-in-time or in batches?
    * If in batches, who owns the inventory in their facility? (Hint: it's almost certainly you)
* If you must hold inventory:
    * What is the lead time on inventory from suppliers? Here, we really care about the longest-lead component.
    * How can you manage demand to keep it in line with your ability to fulfill orders?
    * Are your customers willing to pre-order or tolerate long wait times before receiving the product? 
    * What payment terms will you receive from suppliers? How will this change over time?

## Growth Capital

Of course, hardware businesses also have a major expense in common with software companies: user acquisition. VCs are generally much more comfortable funding this with equity, but it is to the advantage of both founders and investors if you can fund this growth out of operating cash flows. This is where margin comes into play: companies with high margins can plough back more capital into growth, thus avoiding further dilution. 
    
### Key Questions

* What gross margin can you expect on day one? How will this change once you are at scale?
* Are there other significant variable costs associated with selling your product that are not part of COGS (ie. commissions, etc)?
* Can you expect significant volume discounts?
* How will you handle distribution/fulfillment? How does this scale? 

## Supply Chain

Supply chain management poses significant operational challenges that are not usually faced by software businesses. Scaling a supply chain in a high-growth environment can be a monumental task. Initial vendor selection is crucial, but just as important is the ability to predict the points at which you will outgrow your vendors and negotiating new deals well in advance. Of course, this in turn requires you to manage the transitions between vendors all while managing inventory against the backdrop of extreme growth and highly uncertain demand. A deep appreciation for these challenges and a robust plan for addressing them are absolute requirements for any hardware business, but they are double important for those seeking venture funding.

### Key Questions

* Which piece of your supply chain is the bottleneck for:
    * Lead times?
    * Volumes?
* When do you expect to exceed the capacity of your bottleneck?
* How will you increase your capacity when the time comes?
* How much overhead is required to manage your supply chain? Does your team have the experience to handle it?
* Is your supply chain international? If so, how much will customs and/or tariffs impact your business?
* How "deep" is your supply chain? Which vendors will need to talk to each other? How will you/they manage this?
* Who is handling fulfilment? 

