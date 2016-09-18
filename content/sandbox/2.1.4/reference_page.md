---
title_supertext: "Lorem Ipsum"
title: "Nimbi Amorque"
description: ""
project: "sandbox"
project_version: "2.1.4"
menu:
  sandbox-2.1.4:
    name: "Reference"
    identifier: "ref"
    weight: 300
    pre: cloud
toc: true
canonical_link: "https://docs.basho.com/riak/kv/latest/developing"
---

Lorem Markdownum

Lorem markdownum, spem citharam pignora ligavit dantem, folio, **videt**
pericula aera, perfectaque fluens nescitve quoque. Auro sua? Volucrum lacrimis,
si vota altaque: inplerit subit quos _manifesta_, dat emisit fixo tribuam
adnuerat, canum.

Auras seraque, impete! [Suos] nuda frustra latuere in armentum animosque Salmaci
debet quo, dat fateri quae riget ait velari. Casses ut `ut meos conpendia`
ducemque in spernit atque, quid iram **montis**, riget mei! Non idem, Trinacris
mirabile _strenua fuit_ premit neque flammas, uno mentis missa. Et plena
famulasque altera, undis bene damna infirmos timendi et subit tibi!

Notus magnosque Iuppiter est domus concipias tellure matrique dextraeque ad
umbra, dicimus gemitum nomina color: `holus`. Illa moveri sim membris prensantem
fert Cupidinis pubis discenda mortis clamor quarum. Tetigere dixit insula suas
ossibus deos _displicet potest_ aequalique novas silvaque. Quae atque, hoc
nubila comes erit viderat **laborum**?

[Diris sibi] ligno, in illa, indetonsusque meum gradus. Quod **cum et per**
illis cognitus ad captat instructo pererrat misere, in. Vulnere adventu tineae
inmensi `moveoque` pugnacem `legumque alas Capitolia obruit`; tanta adversa. Tua
**Iunonis** arsit mora matre adhuc, pendentia; ego pater fuisset omnes, nec
prole prece prohibent arcus in. Toto Hesperium unam turba illic Echo; adit tua
Parin est seduxit utque subiectum haec adolentur levabas, caede, tui.

[Suos]: http://gestasset.com/rupit.aspx
[Diris sibi]: http://locum.com/


## Pangrams

The quick brown fox jumps over the lazy dog

_The quick brown fox jumps over the lazy dog_

**The quick brown fox jumps over the lazy dog**

**_The quick brown fox jumps over the lazy dog_**

  

Pack my box with five dozen liquor jugs.

_Pack my box with five dozen liquor jugs._

**Pack my box with five dozen liquor jugs.**

**_Pack my box with five dozen liquor jugs._**



## An exhibit of Markdown

Sections selectively taken from <http://www.markitdown.net/markdown>

## Lists

### Ordered list

1. Item 1
2. A second item
3. Number 3
    1. Sub-list
    1. They look like this
    1. Going a bit farther
        1. Two levels deep
        1. Second sub-sub-list
        1. Third
        1. And fourth.
            1. four levels deep
                1. five levels deep
    1. One last element
4. Ⅳ

*Note: the fourth item uses the Unicode character for [Roman numeral four][2].*

[2]: http://www.fileformat.info/info/unicode/char/2163/index.htm

### Unordered list

* An item
* Another item
    * Sub-list
    * With a few items
    * And another item
        * Sub-sub-list
        * Only two items
            * four levels deep
                * five levels deep
* Yet another item
* And there's more...

## Quote

> Here is a quote. What this is should be self explanatory. Quotes are automatically indented when they are used.

Lorem markdownum, spem citharam pignora ligavit dantem, folio, **videt**
pericula aera, per fect aque fluens nescitve quoque. Auro sua? Volucrum lacrimis.

## Note Shortcode

{{% note %}}This is a simple Note, generated with the \{\{% note %\}\} shortcode.{{% /note %}}

Lorem markdownum, spem citharam pignora ligavit dantem, folio, **videt**
pericula aera, per fect aque fluens nescitve quoque. Auro sua? Volucrum lacrimis.


{{% note title="Title Text"%}}This is a note with a title, in addition to wrapped text.{{% /note %}}

Lorem markdownum, spem citharam pignora ligavit dantem, folio, **videt**
pericula aera, per fect aque fluens nescitve quoque. Auro sua? Volucrum lacrimis.


## Headings

There are six levels of headings. They correspond with the six levels of HTML headings. You've probably noticed them already in the page. Each level down uses one more hash character.

### Headings *can* also contain **formatting**

Our anchor generation logic is okay with it, too.

### They can even contain `inline code`

Of course, demonstrating what headings look like messes up the structure of the page.

I don't recommend using more than three or four levels of headings here, because, when you're smallest heading isn't too small, and you're largest heading isn't too big, and you want each size up to look noticeably larger and more important, there there are only so many sizes that you can use.

## H2 -- _Italics_, **Emphasis**, and _**Both**_

**Bold text for scale**. Regular text for scale.

### H3 -- _Italics_, **Emphasis**, and _**Both**_

**Bold text for scale**. Regular text for scale.

#### H4 -- _Italics_, **Emphasis**, and _**Both**_

**Bold text for scale**. Regular text for scale.

##### H5 -- _Italics_, **Emphasis**, and _**Both**_

**Bold text for scale**. Regular text for scale.

###### H6 -- _Italics_, **Emphasis**, and _**Both**_

**Bold text for scale**. Regular text for scale.

## URLs

URLs can be made in a handful of ways:

* A named link to [MarkItDown][3].
* Another named link to [MarkItDown](http://www.markitdown.net/)
* Sometimes you just want a URL like <http://www.markitdown.net/>.

[3]: http://www.markitdown.net/

## Horizontal rule

---

A horizontal rule is a line that goes across the middle of the page.

It's sometimes handy for breaking things up.

## Tables

Parameter | Default | Description
:---------|:--------|:-----------
`r` | `quorum` | How many replicas need to agree when retrieving an existing object before the write
`pr` | `0` | How many [vnodes][glossary vnode] must respond for a read to be deemed successful
`notfound_ok` | `true` | If set to `true`, if the first vnode to respond doesn't have a copy of the object, Riak will deem the failure authoritative and immediately return a `notfound` error to the client

[glossary vnode]: /riak/kv/2.1.4/learn/glossary/#vnode

## Code Blocks

A basic, four-spaces indented codeblock;

    GET /types/<type>/buckets/<bucket>/keys/<key>

Same code, using tripple-backtick fences;

```
GET /types/<type>/buckets/<bucket>/keys/<key>
```

### Tabbed code blocks

Generated using named-fences, one after the other;

```java
// In the Java client, it is best to specify a bucket type/bucket/key
// Location object that can be used as a reference for further
// operations, as in the example below:
Location myKey = new Location(new Namespace("animals", "dogs"), "rufus");
```

```ruby
bucket = client.bucket_type('animals').bucket('dogs')
obj = bucket.get('rufus')
```

```php
$response = (new \Basho\Riak\Command\Builder\FetchObject($riak))
  ->buildLocation('rufus', 'users', 'animals')
  ->build()
  ->execute();
```

```python
bucket = client.bucket_type('animals').bucket('dogs')
obj = bucket.get('rufus')
```

```csharp
// Using the Riak .NET Client it is best to specify a bucket type/bucket/key
// RiakObjectId object that can be used as a reference for further
// operations
var id = new RiakObjectId("animals", "dogs", "rufus");
```

```javascript
client.fetchValue({ bucketType: 'animals', bucket: 'dogs', key: 'rufus' }, function (err, rslt) {
    assert(rslt.isNotFound);
});
```

```erlang
{ok, Obj} = riakc_pb_socket:get(Pid,
                            {<<"animals">>, <<"dogs">>},
                            <<"rufus">>).
```

```golang
cmd, err = riak.NewFetchValueCommandBuilder().
  WithBucketType("animals").
  WithBucket("dogs").
  WithKey("rufus").
  Build()
if err != nil {
    // error occurred
}
```

```curl
curl http://localhost:8098/types/animals/buckets/dogs/keys/rufus
```


