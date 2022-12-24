## Outline for Project

This project is a visual display of the Bitcoin blockchain.

The visuals focus on a few elements of the blockchain's history:

* The minting of new coins. The mint comes from the center, with the coins traveling as a beam of light according to their value (again, interesting to compare as USD vs BTC).

* Coins allocated to the associated wallet over time. The size on screen, and/or brightness, of the wallet will vary with the amount of value held in the wallet. May be interesting to be able to compare how that value changes when calculated solely as Bitcoin, or when calculated as USD according to inflationary value

* Transactions from one wallet to another, represented as an arced line that has a brightness that varies according to amount and may fade over time until very little trace is left

* The creation of wallets. Concentric circles expand outwards with each circle representing one year. Wallets are created around a circle in that year, the new wallets appearing count-clockwise around the circle until the end of the year is reached. 

* There will be a slider bar at the bottom of the screen that shows the progression of time

* This will likely be a movie that can be stopped at any point in time. 

* Interactive objects will be severely limited to only a handful of highly valuable wallets and/or transactions, and they will only be available while their status remains highly relevant on screen. Their interactive nature deactivates after a certain point.

* There might be some interesting trivia that can be activated on the sideline of the wallet, such as a transaction that shows a remarkable exchange hack, or a notable known wallet, etc.

* The final product will have a rasterized "movie screen" type background that plays out over time, with floating interactive objects above it that reveal additional aspects of the story

* The animation should be COOL, as should the effects. Graphic design and illustration time.

* The project is written in C++

* The final project should be able to run over any amount of blocks in the future, although naturally there will be limitations

* Might be nice if there's some type of ongoing animation for new things, showing how they might develop over time before becoming rigid. Eventually, to keep it simple, I'll need them to settle in place.

* Use WASM for web interactivity, I think

To limit the scope and project intensity, and to make calculation more feasible given my available hardware, I will likely have to put a threshold on wallet size. For example, a wallet may have to have held at one point at least $100 USD worth of BTC, or perhaps a minimum BTC amount. Perhaps, only the top 10% or 5% of wallets will remain in calculation over the timeline. If a wallet falls out of that percentage, it becomes a grey dot on the screen or something that is no longer rendered as an interactive SVG object or something.

The final result needs to be an interactive page that is viewable on my web portfolio.

Each wallet would need to have a new element added to the database: the coordinates within the frame that would show where it is located. Searching by those coordinates should be easily achieved, allowing

That's the general concept for now. Realistically, I am aware that this is going to be a behemoth of a project, in part due to the complexity of the code, and in part due to the size of the dataset and resulting processing requirements. 

I'll start with this idea, though, and work my way backwards until I have something I'm pleased with.
