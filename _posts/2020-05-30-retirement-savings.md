---
layout: post
title:  "Retirement Savings 101"
date:   2020-05-30 00:00:00 -0800
author: Guna Prasaad
categories:
---

*Disclaimer: This is a personal note written by the author to clarify the trade-offs within various retirement savings options to self. It is shared only in the public interest that it could be useful to others. It is not intended to serve as an official recommendation either by the author or any associated entities. The author is not a financial advisor in any capacity and provides no guarantee about the factual correctness of any of the following information. However, please reach out if you would like something modified for correctness.*

I recently joined Facebook as a Software Engineer. One of the many things that are thrown at you as you begin settling at your full time job is **Retirement Savings**. As I started reading more, I discovered several retirement savings options - for e.g. traditional 401(k), IRA and their Roth alternatives. While they all share the common purpose of saving for retirement, each one of them is different from the other in a rather subtle way. You can, of course, find several websites and blogposts talking about their similarities and differences such as [this](https://money.usnews.com/money/retirement/articles/retirement-accounts-you-should-consider), [this](https://www.investopedia.com/ask/answers/12/401k.asp) and [this](https://www.schwab.com/ira). Be that as it may, I often found myself unable to answer some key questions about their advantages. I hope to *quantify* the costs and benefits of using these retirement savings accounts.

I will focus only on 4 types of retirement accounts here: traditional and Roth 401(k); traditional and Roth IRA. 

## When you stick to the plan
Fundamentally, there are two kinds of retirement plans based on who sponsors it. 
A 401(k) is a company sponsored retirement plan, while an Individual Retirement Account (IRA) is sponsored by yourself. 
Each company you work at will typically create a 401(k) for you. You can manage an IRA across companies and where you work at has nothing to do with your IRA. 

The unifying constraint in all these types of accounts is that you reap the full benefits when you withdraw money when you retire i.e. after you are $59\frac{1}{2}$ years. Let's look at how simlarities and differences between these different types of accounts when you stick to this plan. 

| Detail                                  | Traditional 401(k)  | Roth 401(k) | Traditional IRA | Roth IRA  |
|-----------------------------------------|---------------------|-------------|-----------------|-----------|
| Employer Contribution Allowed           | Yes                 | Yes         | No              | No        |
| AGI Limit                               | No                  | No          | No              | Yes       |
| Contribution Limit                      | Yes                 | Yes         | Yes             | Yes       |
| Taxed during Contribution               | No                  | Yes         | No              | Yes       |
| Taxed during Withdrawal - Contributions | Yes                 | No          | Yes             | No        |
| Taxed during Withdrawal - Earnings      | Yes                 | No          | Yes             | No        |

Since these are tax advantaged accounts, the IRS has created some checks and balances to prevent abusing them. The first kind is an Adjusted Gross Income (AGI) limit, which applies only to Roth IRA. You are eligible to contribute to a Roth IRA account only if your income is below certain threshold. The second kind of limit is on the amount you can contribute to every financial year. For example, your personal contributions to traditional and Roth 401(k) combined is capped at USD $19,500$; and traditional and Roth IRA combined is capped at USD $6000$ for 2020. You can find up-to-date details elsewhere.

The next major difference is in terms of if and when you pay taxes on contributions and earnings. Contributions to traditional 401(k) or IRA are usually tax deffered and taxed during withdrawal. On the other hand, contributions to Roth 401(k) and IRA are taxed during contribution and is not taxed during withdrawal. Earnings,however, are handled slightly differently. Earnings on contributions in a traditional 401(k) or IRA are taxed during withdrawal, while in case of a Roth 401(k) or IRA, they can be withdrawn tax-free.



It helps to understand a couple of things as we move forward. 
1. **Employer contribution:** The 401(k) accounts are usually supported by your employers and most of them match your contributions upto a certain limit. You can think of this as _extra money_ that you do not get from your employer if you do not contribute. Consider this an incentive by your employer for you to save for your retirement. 
<br>
2. **Tax deferral:** Saving for your retirement is a good thing. And maybe the Government does not want all of you to depend on Social Security for your retirement. So it incentivises you to save for retirement when you can. It does this by letting you _defer_ paying taxes on whatever you save and on whatever that savings grows to in these accounts. However remember 'you have to pay taxes at some point' - if not now, then later. 
<br>
3. **Early withdrawal penalty:** Barring a few exceptional cases, the Government wants you to stick to your plan. These are not your run-of-the-mill savings account. So, they disincentivize you to treat it like one -- by imposing penalties. There is usually a 10% penalty on top of whatever income tax you owe if you withdraw money from these accounts before you are 59.5 years old. Different accounts under different circumstances incur a tax or penalty when withdrawn prematurely, which we will look at in detail below.

If I am always going to pay taxes at some point, then how much is the advantage of these savings accounts really? Is it worth the liquidity that you are giving away? On top of that, $59\frac{1}{2}$ is a good 30 years away and I frankly don't like to look so much ahead. I might want to cash out earlier. Given this uncertainty, how much is the advantage really? Does that mean these investments are totally unattractive? 

Turns out, not exactly! And that is why it helps to quantify the tax and employer benefits that come with these accounts against its limitation. Let us start with a simple question.

## Should you match your employer contribution limit?
Let's say your employer matches $100\%$ upto USD $5000$. We'll see why you should absolutely match the limit in this case! Your post tax earnings at a $30\%$ tax rate would be USD $3500$. But with the employer match, your contribution becomes USD $10000$, and even if you withdraw immediately incurring a penalty of $10\%$, it becomes ~ $(1 - 0.3 - 0.1) * 2 * 5000$ = USD $6000$. 

Precisely, if your employer match ratio is $x$ upto limit USD $y$ and tax ratio $t$, your take home portion corresponding to USD $y$ would be $(1-t)y$ if you do not contribute. If you do and withdraw immediately, it would be $(0.9-t)(1+x)y$. So, it makes sense to contribute when $ (0.9-t)(1+x)y > (1-t)y$
which yields 

$$x > \frac{1}{(9-10t)}$$ 

So, Even for a tax rate as high as $40\%$, you can contribute upto the limit if your employer match is greater than $20\%$.

## Should you contribute more than employer matching limit?
Now, we are done with all the extra money from your employer. The primary advantage of contributing to your retirement accounts now is the tax benefits. How do we quantify this to help with our analysis? Let's define *take home advantage* ($\tau$) as "ratio of take home value when you invest pre-tax income of USD $y$ in one of these accounts to that of investing it elsewhere". Note that this amount, USD $y$, is whatever you contribute beyond your employer matching limit - so no extra money here.

Let's model the scenarios wer are interested in.  Say the current and future tax rates be $t_1$ and $t_2$ and you contribute $y$ USD more than your employer contribution limit. We also assume the net growth rate of principal within or outside the accounts be $g$ i.e. if you invest USD $P$, it grows to $(1+g)P$ during withdrawal however many years later. While this *similar growth* assumption simplifies our analysis, these retirement savings accounts typically have a restricted set of investment options compared to a brokerage account. But we should ideally invest in assets with a similar risk profile and hence similar growth assumption is fine. 

When you invest the money elsewhere in a regular investment account, the take home value of that would be

$$ \left(1 + (1 - t_2) * g\right) * (1 - t_1) * y $$

The take home value at withdrawal for various scenarios in these retirement accounts are summarized below. Compared to Regular denotes the relationship of the take home value with that of a regular investment account. Adjusted growth rate, $\hat{g}$, denotes the effective growth rate for the corresponding type of the retirement account after taking into the account the taxes/penalty due to an early withdrawal. Both of these numbers assume that future tax rate is same as current tax rate $t_1 = t_2$.

**Traditional 401(k) or IRA**
  
| Age                   | Qualified*  | Take Home Value                       | Compared to Regular           | Adjusted Growth Rate  |
|-----------------------|-------------|---------------------------------------|----------------------------------|-----------------------|
| $\geq 59\frac{1}{2}$  | -           | $(1-t_2) * (1+g) * \mathbf{y}$        | Always Greater                   | $g$                   |
| $< 59\frac{1}{2}$     | Yes         | $(1-t_2) * (1+g) * \mathbf{y}$        | Always Greater                   | $g$                   |
| $< 59\frac{1}{2}$     | No          | $0.9 * (1-t_2) * (1+g) * \mathbf{y}$  | Equal when $g = \frac{1}{10t-1}$ | $\frac{9g - 1}{10}$   |


**Roth 401(k) or IRA**
  
| Age                   | 5Y Rule Met? | Qualified  | Take Home Value                                   | Compared to Regular  | Adjusted Growth Rate |
|-----------------------|--------------|------------|---------------------------------------------------|-----------------------------|----------------------|
| $\geq 59\frac{1}{2}$  | Yes          | -          | $(1 + g) * \mathbf{(1-t_1) * y}$                  | Always Greater              | $g$                  |
| $\geq 59\frac{1}{2}$  | No           | -          | $(1 + (1 - t_2) * g) * \mathbf{(1-t_1) * y}$      | Always Equal                | $(1-t) * g$          |
| $< 59\frac{1}{2}$     | Yes          | Yes        | $(1 + g) * \mathbf{(1-t_1) * y}$                  | Always Greater              | $g$                  | 
| $< 59\frac{1}{2}$     | No           | Yes        | $(1 + (1 - t_2) * g) * \mathbf{(1-t_1) * y}$      | Always Equal                | $(1-t) * g$          |              
| $< 59\frac{1}{2}$     | Yes/No       | No         | $(1 + 0.9 * (1-t_2) * g) * \mathbf{(1-t_1) * y}$  | Always $10\%$ Lesser        | $ 0.9(1 - t) * g$    |


### Lower Tax Bracket at Mature Withdrawal
One straightforward upside is if you think you expect your tax rate to be lower during withdrawal than your current tax rate. Assuming you are making a qualified withdrawal during retirement, of course, contributing more is beneficial. But, how much?

For instance, let's say the growth is $500\%$ growth over $30$years (That's not huge! It is approximately a $5.5\%$ YoY compound growth which is quite conservative). So $g=4$. Let's say you pay $35\%$ tax right now and expect to pay $15\%$ when you retire. If you invest USD $1000$ today, then 
* If you save elsewhere, it would grow to a take home of $(0.65 + 4 * 0.85) * 1000 = 4050$
* If you save in a traditional 401(k) or IRA account, you would get $0.85 * 5 * 1000 = 4250$
* If you save in a Roth 401(k) or IRA account, you would get $5 * 0.65 * 1000 = 3250$

Precisely, 

$$ \tau_{\text{TQ}} = \frac{1 + g}{1 + (1-t_2) * g}$$

$$ \tau_{\text{RQ}} = \frac{1 - t_2}{1 - t_1} * \frac{1 + g}{1 + (1-t_2) * g}$$

And more interestingly, it helps to answer the question should you save via a traditional or Roth account and how much do you gain/lose by doing it sub-optimally:

$$ \frac{\tau_{\text{TQ}}}{\tau_{\text{RQ}}} = \frac{1-t_2}{1-t_1}$$

  
### Same Tax Bracket during Withdrawal
In most scenarios barring a few exceptional ones, if you are doing a premature withdrawal, it is considered unqualified and you may have to pay a withdrawal penalty on all or a portion of your savings depending on the type of the account. It is strictly better to leave your savings undisturbed and withdraw only after retirement. However, life is uncertain. You may want to pull the plug. I know this will hurt my take home, but by how much? Certainly there must be an advantage to having my savings grow in a tax advantaged account. When does it break even with investing that money elsewhere and perhaps in a more liquid investment that I can summon to help me during a rainy day?

For this analysis, we will assume that you are in the same tax bracket during withdrawal and you withdraw the entire amount in chunks to belong to the same tax bracket. 

In case of a traditional 401(k) or IRA account, in order to break even with an unqualified withdrawal we want $ 0.9 * (1-t) * (1+g) * y \geq (1 + (1-t) * g) * (1-t) * y$. So, your investment must grow at least

$$ g \geq \frac{1}{10t - 1} $$

in order to break even. In other words, you will not be hurt more than "not saving for retirement using these accounts" if you withdraw your money prematurely after it has grown to $\frac{10t}{10t-1}$ in your traditional 401(k) or IRA account.

For a Roth 401(k) or IRA, there is no break-even if you make an unqualified withdrawal. In fact, you would lose  $$ 0.1 * (1-t) * g * (1-t) * y $$. This is a $10\%$ loss in growth compared to investing the money elsewhere, and a $(10 + 90t)\%$ loss in growth compared to waiting until retirement to take complete advantage of Roth savings. 

However, Roth expands the scope of qualified withdrawals and you should use them when it makes sense. In that case, does it ever make sense to do a qualified withdrawal when the 5-year rule is not met? i.e. You start contributing to a Roth IRA account and withdraw the money in less than 5 years. Yes! In fact, you would exactly break-even with growing your money elsewhere. However, it is sub-optimal -- incurring a loss of $100t\%$ in comparison to waiting to meet the 5-year rule.
