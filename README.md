
## lfemagic

*An IPython extention for LFE (Lisp Flavoured Erlang)*

This work was forked from the HyMagic code by @yardsale8

The `lfemagic` IPython extension allows one to execute hylang code interactively
in a IPython console, qtconsole, or notebook.

### Installation

TBD

### Loading the `lfemagic` extension

#### In a Running IPython

In[1]:

```
%load_ext hymagic
```

#### In an IPython Configuration

TBD

### Executing an LFE cell

You can execute an LFE cell using the `%%lfe magic` as shown below.

In[2]:

```
%%lfe
(defun add1 (n)
    (+ n 1))

(lfe_io:format (add1 5))
```


    6


### Execute an LFE line

You can also use the `%lfe` magic to execute one line of code

In[4]:

```
a = 5
%lfe (sev a (add1 a)) 
a = a + 1
print(a)
```


    7

