# CardSwipeSwift
This repo is a simplified swipe-to-dismiss card style view so you can transition between other views and content. I have modeled it off of various apps and tutorials such as Tinder. My main purpose was to try and simplify the effects of the card style structure by not using pod installs or other dependencies, but doing so without sacrificing a lot of functionality and user experiences such as animations.

I have this listed as a normal file so the best recommenation is just to import the files manually. There is no Cocoapod or Carthage installs for this as I attempted to make this independent from third party dependencies. I may create a pod in the future but as of now just install manually.

The "Card" inside the file (which is listed as a storyCardView) is basically a UIView with a secondary UIView inside, with a label inside that second UIView. The second UIView and label do not serve a purpose for the card-style swiping itself and I encourage you to customize the UIView "Card" to suit your needs.

Tips and Tweeks
The cards are designed to not be dismissed vertically if the main swipe pan guesture is a vertical guesture. The cards will only dismiss from a horizontal guesture to the right or left if the guesture swipe is larger than 200 of the UIView width.You can also custom change this for your needs.
