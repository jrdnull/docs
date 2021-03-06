---
layout: docs
---

# LFE Documentation

## Internal LFE Library

{% highlight text %}
MODULE

        lfe_lib

MODULE SUMMARY

        Lisp Flavoured Erlang (LFE) library

DESCRIPTION

        This module contains a collection of library functions for
        implementing LFE. They are generally not called by the user.

EXPORTS

new_env() -> Environment.

        Create a new environment for the evaluator.

add_env(Env1, Env2) -> Env.

        Add environment Env1 to Env2 such that Env1 shadows Env2.

is_erl_bif(Name, Arity) -> bool().
is_guard_bif(Name, Arity) -> bool().

        Test whether a Name/Arity is a BIF or guard BIF. This works
        for functions and operators.

is_core_form(Name) -> bool().

        Test whether Name is one the LFE core forms.
{% endhighlight %}
