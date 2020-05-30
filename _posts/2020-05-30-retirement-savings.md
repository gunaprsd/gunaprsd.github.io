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

When you invest the money elsewhere, the take home value of that investment is 

$$ \left(1 + (1 - t_2) * g\right) * (1 - t_1) * y $$

The take home value at withdrawal for various scenarios in these retirement accounts are summarized below:

**Traditional 401(k) or IRA**
  
| Age                   | Qualified*  | Take Home Value at Withdrawal         | Regular Account                 | Adjusted Growth Rate  |
|-----------------------|-------------|---------------------------------------|---------------------------------|-----------------------|
| $\geq 59\frac{1}{2}$  | -           | $(1-t_2) * (1+g) * \mathbf{y}$        | Always Greater                  | $g$                   |
| $< 59\frac{1}{2}$     | Yes         | $(1-t_2) * (1+g) * \mathbf{y}$        | Always Greater                  | $g$                   |
| $< 59\frac{1}{2}$     | No          | $0.9 * (1-t_2) * (1+g) * \mathbf{y}$  | Equal when $g = \frac{1}{10t-1} | $\frac{9g - 1}{10}$   |


**Roth 401(k) or IRA**
  
| Age                   | 5Y Rule Met? | Qualified  | Take Home Value at Withdrawal                     | Break Even            | Adjusted Growth Rate  |
|-----------------------|--------------|------------|---------------------------------------------------|-----------------------|-----------------------|
| $\geq 59\frac{1}{2}$  | Yes          | -          | $(1 + g) * \mathbf{(1-t_1) * y}$                  | Always Greater        | $g$                   |
| $\geq 59\frac{1}{2}$  | No           | -          | $(1 + (1 - t_2) * g) * \mathbf{(1-t_1) * y}$      | Always Equal          | $(1-t_2) * g$         |
| $< 59\frac{1}{2}$     | Yes          | Yes        | $(1 + g) * \mathbf{(1-t_1) * y}$                  | Always Greater        | $g$                   | 
| $< 59\frac{1}{2}$     | No           | Yes        | $(1 + (1 - t_2) * g) * \mathbf{(1-t_1) * y}$      | Always Equal          | $(1-t_2) * g$         |              
| $< 59\frac{1}{2}$     | Yes/No       | No         | $(1 + 0.9 * (1-t_2) * g) * \mathbf{(1-t_1) * y}$  | Always $10\%$ Lesser  | $0.9 (1 - t_2) * g$   |


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
