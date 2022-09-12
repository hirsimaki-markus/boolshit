# boolshit - Maybe is the new True. Or False.

_Are you bored of the normal, static booleans? Order now and get Maybe!_

 Maybe is a new boolean type that exists in a superposition of True and False, waiting for its wave function to collapse upon observation. Very similarly to the famous Schrödinger's cat 🐱📦🕵️

# Installation
```shell
pip3 install https://github.com/hirsimaki-markus/boolshit/raw/main/dist/boolshit-1.0.0-py3-none-any.whl
```

# Usage

Any imaginable situation accepting `True` or `False` will accept `Maybe` without a hitch.

```Python
>>> from boolshit import Maybe
>>>
>>> while Maybe: print("Loop is still running!")
...
Loop is still running!
Loop is still running!
Loop is still running!
>>>
>>>
>>> Maybe == Maybe; Maybe == Maybe
True
False
>>>
>>>
>>> 1/Maybe
1.0
>>> 1/Maybe
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
  File "/mnt/c/Users/user/Desktop/maybe.py", line 127, in __rtruediv__
    def __rmul__(_self, other): return other*rnd() # x * M
ZeroDivisionError: division by zero
>>>
>>> # and many more ...
>>>
```

# Motivations behind this act of absurdity? Curiosity and learning.

Consider this project as a practical joke, and academic curiosity, a piece tangible eccentricity. A work of art if you will. With that out of the way, motivations;

* Curiosity, which Maybe killed the cat.
* Academic exercise, that May-e was on the subject of tedium.
* Madness, to which there Maybe was a method.

# Technical

`Maybe` is a singleton instance of the `maybe` class. `Maybe` can be used in any
context that supports the classical, boring, booleans `True` and `False`.
The value of the singleton exists in a superposition of `True` and `False`.
It shall randomly collapse to either one of them upon being observed either
directly or indirectly. The only time `Maybe` will not collapse to boolean
is when it is not operated on. This happens only with plain "Maybe" by
itself (when not in interactive prompt) and with an assignment, e.g.: `x = Maybe`.

This means that `Maybe` can be assigned as is and it will be both `True` and
`False` until the assigned variable is coerced to some other type. In
essence this means that you can but `Maybe` into any imaginable context
and it will behave exactly as `True` or `False`, depending on your luck.

`Maybe` obeys the limitations of a singleton pattern. `Maybe is Maybe` will
always be `True`, while `Maybe == Maybe` is determined upon observation.

Below is a list of some example contexts that will accept Maybe, Both
left hand and right hand operations will work as one might expect.

# Technical jargon

`bool` can not be subclassed with reasonable effort, so
`maybe` is a subclass of `int`, as is `bool`. Maybe achieves compatibility by
defining a counterpart to every method and attribute of booleans. While
strictly not `bool`, `maybe` class and its instance, `Maybe` is a boolean in
the practical sense. It acts like a duck, it quacks like a duck, and thus it
is a duck.
