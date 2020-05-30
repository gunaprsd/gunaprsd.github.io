---
layout: post
title:  "Retirement Savings 101"
date:   2020-05-30 00:00:00 -0800
categories:
---
I recently joined Facebook as a Software Engineer. One of the many things that are thrown at you as you begin settling at your new full time job is **retirement savings**. As I started reading more, I learnt about several retirement savings instruments such as the traditional 401(k), IRA and their Roth alternatives. While they all share the common purpose of saving for retirement, each one of them is different from the other in a rather subtle way. You can, of course, find several websites and blogposts talking about their similarities and differences such as this, this and this. But I often found myself unable to _quantify_ their advantages and disadvantages. I hope to discover the answers to some of them via this post.

It helps to understand a couple of things before we move forward. 
1. **Employer contribution:** The 401(k) accounts are usually supported by your employers and most of them match your contributions upto a certain limit. You can think of this as _extra money_ that you do not get from your employer if you do not contribute. Consider this an incentive by your employer for you to save for your retirement. 
<br>
2. **Tax deferral:** Saving for your retirement is a good thing. And maybe the Government does not want all of you to depend on Social Security for your retirement. So it incentivises you to save for retirement when you can. It does this by letting you sometimes _defer_ paying taxes on whatever you save and on whatever that savings grows to in these accounts. However remember 'you have to pay taxes at some point' - if not now, then later. Then, how much is the advantage really, you ask? I had the same question and maybe you will find the answer here. Read on.
<br>
3. **Early withdrawal penalty:** Barring a few exceptional cases, the Government wants you to stick to your plan. These are not your run-of-the-mill savings account. So, they disincentivize you to treat it like one -- by imposing penalties. There is usually a 10% penalty on top of whatever income tax you owe if you withdraw money from these accounts before you are 59.5 years old. For me, 59.5 is a good 35 years ahead and I frankly don't like to look so much ahead. And I might want to cash out earlier. Does that mean these instruments are totally unattractive? Not exactly. And that is why it helps to quantify the above two incentives against this limitation. 
  

## Account Types
I will limit the discussion in this post to 4 types of retirement savings accounts - traditional and Roth 401(k); traditional and Roth IRA. I have tried to summarize their differences in this table. 

| Detail | Traditional 401(k) | Roth 401(k) | Traditional IRA | Roth IRA |
|--------|--------------------|-------------|-----------------|----------|
| Employer Contribution Allowed | Yes | Yes | No | No |
| AGI Limit | No | No  | No | Yes |
| Contribution Limit | Yes | Yes | Yes | Yes |
| Tax Deferral on Contribution | Yes | No | Yes | No |
| Taxed during Withdrawal - Contributions | Yes | No | Yes | No |
| Taxed during Qualified Withdrawal - Earnings | Yes | No | Yes | No |
| Taxed during Unqualified Withdrawal - Earnings | Yes | Yes | Yes | Yes |
| Unqualified Withdrawal Penalty - Contributions | Yes | No | Yes | No |
| Unqualified Withdrawal Penalty - Earnings | Yes | Yes | Yes | Yes |

To be eligible to use Roth IRA, your Adjusted Gross Income (AGI) must be less than a certain limit; others do not have such a limit. Since all these are tax advantaged accounts, they also have a limit on how much you can contribute to them. For example, your personal contributions to traditional and Roth 401(k) combined is capped at $19,500 for 2020. 

Then comes the major difference between traditional and Roth accounts in terms of when you pay taxes on contributions and if it incurs unqualified withdrawal penalty. Contributions to traditional 401(k) or IRA are tax deferred, and are taxed during withdrawal. Additionally, if the withdrawal is unqualified, it also incurs a penalty. On the other hand, contributions to Roth 401(k) and IRA are post-tax. Since you have paid taxes now, you do not have to pay taxes or penalty when you withdraw the contribution amount.

The other major difference is in terms of how earnings are handled. Earnings on contributions in traditional 401(k) or IRA are taxed during withdrawal and also incur a penalty if done prematurely. In case of a Roth 401(k) or IRA, if the withdrawal happens after maturity, the earnings are both penalty and tax-free. However in case of an unqualified withdrawal, earnings is both taxed and penalized.

Now, it is time to dive deeper and quantify these. 
  

## Should you match your employer contribution limit?
Let's say your employer matches $100\%$ upto USD $5000$. We'll see why you should absolutely match the limit in this case! Your post tax earnings at a $30\%$ tax rate would be USD $3500$. But with the employer match, your contribution becomes USD $10000$, and even if you withdraw immediately incurring a penalty of $10\%$, it becomes ~ $(1 - 0.3 - 0.1) * 2 * 5000$ = USD $6000$. 

Precisely, if your employer match ratio is $x$ upto limit USD $y$ and tax ratio $t$, your take home portion corresponding to USD $y$ would be $(1-t)y$ if you do not contribute. If you do and withdraw immediately, it would be $(0.9-t)(1+x)y$. So, it makes sense to contribute when $ (0.9-t)(1+x)y > (1-t)y$
which yields 

$$x > \frac{1}{(9-10t)}$$ 

So, Even for a tax rate as high as $40\%$, you can contribute upto the limit if your employer match is greater than $20\%$.

## Should you contribute more than employer matching limit?
Now, we are done with all the extra money from your employer. The primary advantage of contributing to your retirement accounts now is the tax benefits. How do we quantify this to help with our analysis? Let's define *take home advantage* ($\tau$) as "ratio of take home value when you invest pre-tax income of USD $y$ in one of these accounts to that of investing it elsewhere". Note that this amount, USD $y$, is whatever you contribute beyond your employer matching limit - so no extra money here.

Let's model the scenarios wer are interested in.  Say the current and future tax rates be $t_1$ and $t_2$ and you contribute $y$ USD more than your employer contribution limit. We also assume the net growth rate of principal within or outside the accounts be $g$ i.e. if you invest USD $P$, it grows to $(1+g)P$ during withdrawal however many years later. While this *similar growth* assumption simplifies our analysis, these retirement savings accounts typically have a restricted set of investment options compared to a brokerage account. But we should ideally invest in assets with a similar risk profile and hence similar growth assumption is fine. 


| Scenario                                        | Take Home Value at Withdrawal                     |
|-------------------------------------------------|---------------------------------------------------|
| Not Contribute                                  | $\left((1-t_1) + (1-t_2) * g\right) * \mathbf{y}$ |
| Traditional 401(k)/IRA - Qualified Withdrawal   | $(1-t_2) * (1+g) * \mathbf{y}$                    |
| Traditional 401(k)/IRA - Unqualified Withdrawal | $0.9 * (1-t_2) * (1+g) * \mathbf{y}$              |
| Roth 401(k)/IRA - Qualified Withdrawal          | $(1+g) * \mathbf{(1-t_1) * y}$                    |
| Roth 401(k)/IRA - Unqualified Withdrawal        | $(1 + 0.9 * (1-t_2) * g) * \mathbf{(1-t_1) * y} $ |

### Lower Tax Bracket during Withdrawal
One straightforward upside is if you think you expect your tax rate to be lower during withdrawal than your current tax rate. If you are making a qualified withdrawal, of course, contributing more is beneficial. But, how much more?

$$ \tau_{\text{TQ}} = \frac{(1-t_2) * (1+g)}{\left((1-t_1) + (1-t_2) * g\right)}$$

### Same Tax Bracket during Withdrawal

## Should you contribute more with your post-tax money?
