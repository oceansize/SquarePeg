# Premise for GapFiller 

### The problem

Media owners such as The Telegraph or Clear Channel make their money by selling space, be it a billboard, space in a magazine/newspaper or screen time at the beginning of a cinema broadcast.

However, sometimes due to various factors these companies can end up with unallocated space at the end of the day/week/month - say for example it has been a slow sales period, or a previously-committed client drops out. This puts the media owner in a compromised position, and they end up needing to sell off the advertising space quickly. This is known as **'short term'**.

Due to the last-minute nature of the situation, the media owner expects the client to come up with suitable artwork to fill the space at very short notice.  In exchange for this inconvenience, the advertising space is sold off at a massive discount making it an extremely lucrative option for, say, an advertising agency who can supply the artwork on time. They charge their client for the space with a decent amount of markup and make a lot more profit than they usually would on an advertising campaign.

This does leave the media owner in a precarious situation though - if they offer the space to a client who fails to deliver the artwork on time, then the media owner loses out on potential revenue, whilst also having nothing displaying in their media location, which devalues their product and puts clients in a stronger position when it comes to agreeing future prices.

The advertising agency also has a problem, because clients are generally unreasonable in their expectations and care very little about deadlines, as that is "the agency's problem".

Therefore, both agency and media owner want to offer the short term to clients who are likely to have artwork that is either ready to go immediately, OR has artwork that can be easily adapted to fit the requirements of the space.

### Enter GapFiller

I propose an application that can take the specification of some advertising space, and compare existing client's artwork history (and other trends) to assess their risk factor when offering short term. Currently nothing seems to exist to fulfil this need.

### Most Viable Product

The most immediately useful software that one could come up with in this context is something that compares the specifications of the ad space, with existing artwork. Drilling down even more, looking at the aspect ratio of say, a newspaper ad and comparing it with the dimensions of a piece of artwork would be enough to get started. If the problem this would solve is a little tricky to understand, perhaps an example would help:

![](https://github.com/roidriscoll/GapFiller/blob/master/images/AdExample.gif?raw=true)

In the animated example above, our youthful user will have identified that option #4 is by far and away the best fit for the ad space, and thus involves the least work to turn that artwork around quickly for maximum win.

### App Outline

I would suspect that the basic functionality of comparing a Height x Width ratio against instances of artwork in a database would be relatively simple, and as an MVP I think it's extremely achievable.

We could then extend the app to take into account how old the artwork in the database is, perhaps even allow the option to categorize artwork by campaign or other such relevant data.

### Smart Image Recognition

As it stands the app would be incredibly useful for most agencies and media owners. However, an experienced Artworker can look at an ad and guestimate how much work it will be to convert artwork from one aspect ratio to another. If we had image recognition that could potentially identify blocks such as booking details, title treatments and faces, we would have an unbeatable product.

While this might sound a little unreachable, I would like to point you to a javascript library which automatically crops photos based on detecting dominant contrast in an image:

[Focal Point (article on
DesignShack.com)](https://raw.githubusercontent.com/roidriscoll/GapFiller/master/images/AdExample.gif?token=ACI6tTDFnX2II0-fl7C7jtMkpqCOFjnaks5WWxIiwA%3D%3D)

### Proposed Stack

Whatever floats your boat.
