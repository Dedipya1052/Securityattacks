# Poisoned tenants
ID: SAT1030

## Tactics
* Initial Access

## Summary

An adversary can register a new tenant that it controls and administers with the intent of tricking users to join it, by convincing them it is owned by their organization.

This often means the adversary will have access to all data within the SaaS tenant and may be able to abuse employee-created OAuth or API integrations with other SaaS apps. Targeting SaaS apps that require or encourage users to create integrations with sensitive assets (such as their mailbox) during signup are more likely to yield useful data for the adversary.

In many cases, execution of such an attack will take careful social engineering. However, invite functionality and automatic account association features often found in SaaS apps can make this attack easier to perform. Some SaaS vendors even automatically prompt a user to join a tenant when they sign up to the app if an invite has previously been sent (even if they ignored the invitation itself) increasing the longevity and chance of a successful attack.

Adversaries may use other techniques to make poisoned tenants appealing to users, such as upgrading the tenant to a higher license tier, unlocking useful features.

A demo video of an attack chain combining a poisoned tenant with a [SAMLjacking](/techniques/samljacking/description.md) attack is given below:
 
[![demo video](https://img.youtube.com/vi/4gAeSxbycXU/0.jpg)](https://www.youtube.com/watch?v=4gAeSxbycXU)

## Examples
* [Trello](examples/trello.md)
* [Nuclino](examples/nuclino.md)

## References
* [SAMLjacking a poisoned tenant - Technical blog post](https://pushsecurity.com/blog/samljacking-a-poisoned-tenant/)
