---
layout: post
title:      "Never be afraid to make a come back"
date:       2021-02-09 19:26:30 -0500
permalink:  never_be_afraid_to_make_a_come_back
---


Long time, no see, Flatiron.

After 2020 being, well, 2020, I came back to finish what I started. Taking a break gave me perspective.

I work at software company that support businesses who have been very directly affected by the pandemic. Over 20% of our clients closed their doors forever. Seeing how quickly those businesses closed and how 35% of our own work force was lost in one day, it made me take a moment and think about what endures in such a situation.

Economies change. Markets rally and crash.

Thus, as the saying goes, the only constant is change. Our greatest teacher truly is experience.

And in that vein, I want to encourage all those struggling right now: in life, in the curriculum, in whatever is on your plate. Keep putting one foot in front of the other. The lessons learned teach a skill. 

> Skills cannot be lost. They are only surrendered.


`- - - - - - - - ALL YOUR CODE ARE BELONG TO US - - - - - - - - `



*On to the coding part of this little post.*

The most recent assignment that I struggled with was the Tic Tac Toe with AI. Ironically, it wasn't the conditional that got me. It was the nuts and bolts of the actual Tic Tac Toe game.

The culprit?

`nil` vs `false`

```
My code was largely in line, until the very end...
  def won?
    WIN_COMBINATIONS.each do |win_combination|
      # lots of code here
      end
    end
    nil
  end
```

That little part at the end....where is says nil? Did it throw an error?

Not directly. It passed the other tests I did prior to that moment. 

The error was being thrown on this line of code instead:

```
if self.won?
puts "Congratulations " + self.winner + "!"
end
```

The `self.winner` kept throwing an error saying that i*t could not reconcile the conditional*. Reading those error messages did eventually pay off, but it led to me a part of the assignment I did not anticipate. `nil` and `false` are different, was the lesson. Two hours later....the `nil` was at last replaced and the program worked.

Other lessons learned....in the event you've been away for awhile, remember that `learn save` will save updates to your program. Another two hours would have been saved if not for my edits in the IDE not being pushed to my github.

Again, the best teacher turns out to be experience. Have a forgotten since then? No.


> I hope my example leaves an imprint to save early, save often and remember that `nil` and `false` are not necessarily interchangeable.
