# boolshit - Maybe is the new True. Or False.

_Are you bored of the normal, static booleans? Order now and get Maybe!_

 Maybe is a new boolean type that exists in a superposition of True and False, waiting for its wave function to collapse upon observation. Very similarly to the famous Schrödinger's cat 🐱📦🕵️

# Installation
From PyPi:
```shell
pip3 install boolshit
```
From repository:
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
* Academic exercise, that Maybe was on the subject of tedium.
* Madness, to which there Maybe was a method.

# Technical

`Maybe` is a singleton instance of the `maybe` class. `Maybe` can be used in any
context that supports the classical, boring, booleans `True` and `False`.
The value of the singleton exists in a superposition of `True` and `False`.
It shall randomly collapse to either one of them upon being observed either
directly or indirectly. The only time `Maybe` will not collapse to boolean
is when it is not operated on. This happens only with plain `Maybe` by
itself (when not in interactive prompt) and with an assignment, e.g.: `x = Maybe`.

This means that `Maybe` can be assigned as is and it will be both `True` and
`False` until the assigned variable is coerced to some other type. In
essence this means that you can put `Maybe` into any imaginable context
and it will behave exactly as `True` or `False`, depending on your luck.

`Maybe` obeys the limitations of a singleton pattern. `Maybe is Maybe` will
always be `True`, while `Maybe == Maybe` is determined upon observation.

# Technical jargon

`bool` can not be subclassed with reasonable effort, so
`maybe` is a subclass of `int`, as is `bool`. Maybe achieves compatibility by
defining a counterpart to every method and attribute of booleans. While
strictly not `bool`, `Maybe` is a boolean in
the practical sense. It acts like a duck, it quacks like a duck, and thus it
is a duck.

# A most beautifully formatted piece of art

**Q:** Why would you paste source code here? _ALSO, WHAT DID YOU DO TO THE FORMATTING?!_

**A:** It's called art. This source is beyond being production ready. It is museum ready.
Also, documenting a handy list of magic methods.

```Python
#!/usr/bin/env python3
"""Full source, minified."""
from random import choice
rnd = lambda: choice((True, False))
class maybe(int):
    def __bool__(_self): return rnd() # bool(M) [builtins section begin]
    def __pos__(_self): return +(rnd()) # +M
    def __neg__(_self): return -(rnd()) # -M
    def __invert__(_self): return ~(rnd()) # ~M
    def __abs__(_self): return abs(rnd()) # abs(M)
    def __repr__(_self): return str(rnd()) # repr(M)
    def __str__(_self): return str(rnd()) # str(M)
    def __int__(_self): return int(rnd()) # int(M)
    def __float__(_self): return float(rnd()) # float(M)
    def __ceil__(_self): return rnd() # math.ceil(M)
    def __floor__(_self): return rnd() # math.floor(M)
    def __trunc__(_self): return int(rnd()) # math.trunc(M)
    def __add__(_self, other): return rnd() + other # M+x
    def __radd__(_self, other): return other + rnd() # x+M
    def __mul__(_self, other): return rnd()*other # M*x
    def __rmul__(_self, other): return other*rnd() # x*M
    def __pow__(_self, other): return rnd() ** other # M**x
    def __rpow__(_self, other): return other ** rnd() # x**M
    def __rshift__(_self, other): return rnd() >> other # M>>x
    def __rrshift__(_self, other): return other >> rnd() # x>>M
    def __lshift__(_self, other): return rnd() << other # M<<x
    def __rlshift__(_self, other): return other << rnd() # x<<M
    def __mod__(_self, other): return rnd() % other # M%x
    def __rmod__(_self, other): return other % rnd() # x%M
    def __truediv__(_self, other): return rnd() / other # M/x
    def __rtruediv__(_self, other): return other / rnd() # x/M
    def __floordiv__(_self, other): return rnd() // other # M//x
    def __rfloordiv__(_self, other): return other // rnd() # x//M
    def __sub__(_self, other): return getattr(rnd(), "__sub__")(other) # M-x
    def __rsub__(_self, other): return getattr(rnd(), "__rsub__")(other) # x-M
    def __index__(_self): return int(rnd()) # oct,bin,hex(M), [1,2,3][M]
    def __round__(_self, *a): return getattr(rnd(), "__round__")(*a) # round(M)
    def __format__(_self, f): return getattr(rnd(), "__format__")(f) # .format
    def __and__(_self, other): return getattr(rnd(), "__and__")(other) # M&x
    def __rand__(_self, other): return getattr(rnd(), "__rand__")(other) # x&M
    def __or__(_self, other): return getattr(rnd(), "__or__")(other) # M|x
    def __ror__(_self, other): return getattr(rnd(), "__ror__")(other) # x|M
    def __xor__(_self, other): return getattr(rnd(), "__xor__")(other) # M^x
    def __rxor__(_self, other): return getattr(rnd(), "__rxor__")(other) # x^M
    def __lt__(_self, other): return getattr(rnd(), "__lt__")(other) # M<x
    def __le__(_self, other): return getattr(rnd(), "__le__")(other) # M<=x
    def __eq__(_self, other): return getattr(rnd(), "__eq__")(other) # M==x
    def __ne__(_self, other): return getattr(rnd(), "__ne__")(other) # M!=x
    def __ge__(_self, other): return getattr(rnd(), "__ge__")(other) # M>=x
    def __gt__(_self, other): return getattr(rnd(), "__gt__")(other) # M>x
    def __divmod__(_self, other): return divmod(rnd(), other) # divmod(M, x)
    def __rdivmod__(_self, other): return divmod(other, rnd()) # divmod(x, M)
    def from_bytes(*_, **__): return rnd() # [int() section begin]
    def conjugate(_self): return int(rnd())
    def bit_length(_self): return (rnd()).bit_length()
    def as_integer_ratio(_self): return (rnd()).as_integer_ratio()
    def to_bytes(self, *a, **kwa): return getattr(rnd(), "to_bytes")(*a, **kwa)
    def __hash__(_s): return int(rnd()) # hash(M) ----[class meta section]----
    def __getnewargs__(_self): return (None, ) # for pickling
    def __dir__(_self): return getattr(rnd(), "__dir__")() # dir(M)
    def __reduce__(_self): return getattr(rnd(), "__reduce__")() # pickling
    def __delattr__(self, name): object.__delattr__(self, name) # obj del
    def __init_subclass__(_self): return getattr(rnd(), "__init_subclass__")()
    def __setattr__(self, name, value): object.__setattr__(self, name, value)
    def __reduce_ex__(_self, p): return getattr(rnd(), "__reduce_ex__")(p)
    def __init__(s): maybe.S = s; maybe.__new__ = lambda _:maybe.S # singleton
    def __getattribute__(s, atr): # shadow attributes protected on C level
        prot = ("real", "numerator")
        return int(rnd()) if atr in prot else object.__getattribute__(s, atr)

Maybe = maybe()  # Actual Maybe boolean
```
