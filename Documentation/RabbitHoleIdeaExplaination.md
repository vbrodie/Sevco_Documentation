# URL Structure

So basically our current website structure for our platform is:

`www.website.com/your-id/subpage`

The `your-id` slug should be replaced with whatever name you designated for your account when you initially signed up. `subpage` is whatever page on the platform you are visiting. For example:

`www.website.com/sploot/buy-treatos`

## The Sole Permalink

A **permalink** is a link that is static and takes you to a website / page on a website no matter what. In the case of this platform, there's some fun **API** calls behind the scene to identify what account you are already logged into. 

Currently there is no **permalink** for any of the pages on the platform _expect_ the **Homepage**. The **permalink** for the **Homepage** is `www.website.com`. Meaning if you were to type `www.website.com/your-id` without a `sub-page` specified, it would take you to `www.website.com` by default.


# The Problem

Because only the **Homepage** has a **permalink**, all other pages must contain `/your-id/` for your browser to direct you to them. For example, the **Settings** and **Profile** page must be entered link this:

`www.website.com/your-id/settings`
`www.website.com/your-id/profile`

If you were to type in `www.website.com/settings` it would take you to the **Homepage** (`www.website.com`) be default, because the `/your-id/` slug was not specified and the Homepage is the only page with a **permalink** in the platform.

# Solution

We create **permalinks** for every page in the platform. This would mean that the same behind-the-scenes **API** calls that allow the **Homepage** to have a permalink would also be done for other pages on the platform. 

So, instead of having to type:

`www.website.com/sploot/buy-treatos`

You could type:

`www.website.com/buy-treatos`

# Why Tho?

Because I want to be able to link to specific pages in the platform. This can't currently be done because the `your-id` slug is unique for each user.

If somebody logged into the account `blep` were to go to visit `www.website.com/sploot/buy-treatos`, the platform would basically ignore everything after `www.website.com` because the account `sploot` could not be validated.

If there were a **permalink** (`www.website.com/buy-treatos`), Comrade could access the treato store from whatever account he was logged into.
