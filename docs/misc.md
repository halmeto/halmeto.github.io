---
layout: default
title: Miscellaneous
permalink: /misc/
---

This page lists various hobby projects I've been working on. At the moment they are mostly related to basketball, so a diversification of the portfolio in this regard could be in order.

**Four Factors Revisited**

In basketball, a rough ''fingerprint'' of a team's offensive performance is given by the Four Factors (originally due to Dean Oliver): 
- effective field goal percentage (eFG%)
- turnover rate (TOV%)
- offensive rebound rate (ORB%)
- free throw rate (FTr). 

These may sound somewhat arbitrary. Why these four specifically stems from the fact that they quantify (mostly) very separate facets of basketball offense, but at the same time cover all the ways a possession can end. If you are a statistician who is very lost, you can think of them as the principal components of basketball offense. Everyone knows and uses the four factors now, but what is interesting is that they indeed are (almost) a [''sufficient statistic''](https://en.wikipedia.org/wiki/Sufficient_statistic) for the offensive efficiency (points scored per possession) of a team. That is, if you know the values of the four factors, you can (almost) calculate the offensive efficiency (ORTG) of the team directly. The formula is not so ugly: 

$$
    \text{Offensive Efficiency} \approx (1 - \text{TOV%}) \frac{2\,\text{eFG%} + \text{FTr}}{1- \text{ORB%} (1 - \text{FG%}) + \mu \, \frac{\text{FTr}}{\text{FT%}}}.
$$

As you can see, one needs a couple more things besides just the four factors for the actual number, but the practical impact of them is small. For a full explanation of what this all means and what it could be used for, see the [pre-print](https://arxiv.org/abs/2305.13032) we wrote with Jirka Poropudas. A very cool implementation of the formula as an interactive calculator can be found at [databallr.com](https://databallr.com/calculator). 

**Korisliigamanageri**

Everyone had a new hobby during COVID, and my very boring one was trying to understand how one builds a website. These days you do this by talking to a chatbot, back then one watched youtube tutorials. The end result was a [fantasy basketball manager game](https://korisliigamanageri.net/) for the Finnish basketball league. Unlike most COVID hobbies, this one still somewhat exists, with between 400-600 users signing up yearly for the game for 5 years running, which, in the context of Finnish basketball, is not too bad. Thankfully, the game requires minimal maintenance.


