
# Microsoft 365 docs navigation guide

This topic provides some tips and tricks for navigating the Microsoft 365 technical documentation space.  

## Impact to customers who don't transition

The following table summarizes the impact to customers who don't transition from a Microsoft 365 Business Preview subscription to a Microsoft 365 Business subscription.

|       | T-0 to T+30     | T+30 to T+60 | T+60 to T+120 | Beyond T+120  |
|-------|-----------------|--------------|---------------|---------------|
| **State** | In grace period | Expired      | Disabled      | Deprovisioned |
| **Service impacts**                                                        |
| **Microsoft 365 Business admin portal** | No impact to functionality | No impact to functionality | Can add/delete users, purchase subscriptions. Can't assign/revoke licenses. | Customer's subscription and all data is deleted. Admin can manage other paid subscriptions. |
| **Office apps**                         | No end user impact | No end user impact | Office enters reduced functionality mode. Users can view files only. | Office enters reduced functionality mode.Users can view files only. |
| **Cloud services (SharePoint Online, Exchange Online, Skype, Teams, and more)** | No end user impact | No end user impact | End users and admins have no access to data in the cloud. | Customer's subscription and all data are deleted. |
| **EM+S components** | No admin impact No end user impact | No admin impact No end user impact | Capability is no longer enforced. See [Mobile device impacts upon subscription expiration](#mobile-device-impacts-upon-subscription-expiration) and [Windows 10 PC impacts upon subscription expiration](#windows-10-pc-impacts-upon-subscription-expiration) for more info. | Capability is no longer enforced. See [Mobile device impacts upon subscription expiration](#mobile-device-impacts-upon-subscription-expiration) and [Windows 10 PC impacts upon subscription expiration](#windows-10-pc-impacts-upon-subscription-expiration) for more info. |
| **Windows 10 Business** | No admin impact No end user impact | No admin impact No end user impact | Capability is no longer enforced. See [Mobile device impacts upon subscription expiration](#mobile-device-impacts-upon-subscription-expiration) and [Windows 10 PC impacts upon subscription expiration](#windows-10-pc-impacts-upon-subscription-expiration) for more info. | Capability is no longer enforced. See [Mobile device impacts upon subscription expiration](#mobile-device-impacts-upon-subscription-expiration) and [Windows 10 PC impacts upon subscription expiration](#windows-10-pc-impacts-upon-subscription-expiration) for more info. |
| **Azure AD login to a Windows 10 PC** | No admin impact No end user impact | No admin impact No end user impact | No admin impact No end user impact | Once the tenant is deleted, a user can sign in with local credentials only. Re-image the device if there are no local credentials. |

## Hub page

The Microsoft 365 hub page can be found at [https://aka.ms/microsoft365docs](https://aka.ms/microsoft365docs) and is the entry point for finding relevant Microsoft 365 content.

You can always navigate back to this page by selecting **Microsoft 365** from the header at the top of every page within the Microsoft 365 technical documentation set:

# JupyterLab Demo Start

JupyterLab: The next generation user interface for Project Jupyter

https://github.com/jupyter/jupyterlab

It started as a collaboration between:

* Project Jupyter
* Bloomberg
* (then) Continuum

| asfasdfasdfasdf   | asdfasdf  | asdfasdf  | asdfasdfasdf  | asdfasdfasdfasdf  |
|-----------------  |---------- |---------- |-------------- |------------------ |
| 1324              | 2         | 2         | 1             | 1                 |
| 1234              | 2         | 2         | 1             | 1                 |
| 1234              | 2         | 2         | 2             | 1                 |

## Tables

First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column

and now involves many other<sup>[1](#footnote_1)</sup>  people from many other places (not purely academic or business)

<a name="footnote_1">1</a>: 주석

```javascript
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
```


## 1) Building blocks of interactive computing

### Start with the launcher


Use it to open different activities:

* Notebook
* Console
* Editor
* Terminal

### Notebooks

* Open example notebooks to show that notebooks still work
* Collapse input/output
* Drag and drop cells

### Demonstrate left panel plugins:

* File Browser (file operations, context menu, including drag and drop)
* Running
* Command Palette (fuzzy searching for 'new')

### Markdown example

* Open `markdown_python.md` in the File Editor
* View the rendered markdown, arrange side by side
* Attach a Kernel/Console and run the code by selecting blocks and pressing
  `Shift+Enter`

### Arrange the building blocks in the main area

The dock panel allows you to arrange the activites into an
arbitrary layout.

Tabs and single document mode allow you to focus.

## 4) File handlers

JupyterLab has a powerful and extensible architecture for handling a wide range of file formats:

* CSV
  - `./data/iris.csv` (small)
  - `TCGA_Data` (small to medium)
  - Urban_Data_Challenge: `data/big.csv`
* Images
  - `data/hubble.png`
* Vega-Lite
  - `data/vega.vl.json`
* Open DC museum GeoJSON file from [OpenData DC](http://opendata.dc.gov/datasets/2e65fc16edc3481989d2cc17e6f8c533_54): `data/Museums_in_DC.geojson`
* Notebook demonstrating bqplot widgets: `notebooks/bqplot.ipynb`

## 5) Find and Replace
first class support for find and replace across JupyterLab, currently supported in 
notebooks and text files and is extensible for other widgets who wish to support it.

## 6) Status Bar
We have integrated the JupyterLab Status Bar package package into the core distribution. Extensions can add their own status to it as well 

## 7) Printing

A printing system allows extensions to customize how documents and activities are printed. 

## 8) JupyterHub

We now include the JupyterHub extension as a core JupyterLab extension, so you no longer need to install @jupyterlab/hub-extension (supporting multi-user + authentication workflows)

## 9) Plugin architecture

The genius of open-source is being able to shape your tools to your heart's content.

Just like Jupyter is built on top of building blocks of the protocol and message spec, *you* can build on this platform for your workflow.

* Everything in JupyterLab is an extension, including everything we have demoed
* Extensions are just `npm` packages with metadata
* Anyone can create, package, ship plugins
* Extension can, for example:
  - Add things to command palette, menu
  - Add viewers for documents
  - Expose other controls (e.g., manage a spark cluster?)
  - Provide more capabilities to the system

## What will you build?


# Markdown

Sphinx can be configured to use markdown using the [recommonmark](https://github.com/readthedocs/recommonmark)
extension. recommonmark is strict and does not natively support tables or common extensions
to markdown.

---


## Body copy

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras arcu libero,
mollis sed massa vel, *ornare viverra ex*. Mauris a ullamcorper lacus. Nullam
urna elit, malesuada eget finibus ut, ullamcorper ac tortor. Vestibulum sodales
pulvinar nisl, pharetra aliquet est. Quisque volutpat erat ac nisi accumsan
tempor.

**Sed suscipit**, orci non pretium pretium, quam mi gravida metus, vel
venenatis justo est condimentum diam. Maecenas non ornare justo. Nam a ipsum
eros. [Nulla aliquam](#) orci sit amet nisl posuere malesuada. Proin aliquet
nulla velit, quis ultricies orci feugiat et. `Ut tincidunt sollicitudin`
tincidunt. Aenean ullamcorper sit amet nulla at interdum.

## Headings

### The 3rd level

#### The 4th level

##### The 5th level

###### The 6th level

## Headings <small>with secondary text</small>

### The 3rd level <small>with secondary text</small>

#### The 4th level <small>with secondary text</small>

##### The 5th level <small>with secondary text</small>

###### The 6th level <small>with secondary text</small>

## Blockquotes

> Morbi eget dapibus felis. Vivamus venenatis porttitor tortor sit amet rutrum.
  Pellentesque aliquet quam enim, eu volutpat urna rutrum a. Nam vehicula nunc
  mauris, a ultricies libero efficitur sed. *Class aptent* taciti sociosqu ad
  litora torquent per conubia nostra, per inceptos himenaeos. Sed molestie
  imperdiet consectetur.

### Blockquote nesting

> **Sed aliquet**, neque at rutrum mollis, neque nisi tincidunt nibh, vitae
  faucibus lacus nunc at lacus. Nunc scelerisque, quam id cursus sodales, lorem
  [libero fermentum](#) urna, ut efficitur elit ligula et nunc.

> > Mauris dictum mi lacus, sit amet pellentesque urna vehicula fringilla.
    Ut sit amet placerat ante. Proin sed elementum nulla. Nunc vitae sem odio.
    Suspendisse ac eros arcu. Vivamus orci erat, volutpat a tempor et, rutrum.
    eu odio.

> > > `Suspendisse rutrum facilisis risus`, eu posuere neque commodo a.
      Interdum et malesuada fames ac ante ipsum primis in faucibus. Sed nec leo
      bibendum, sodales mauris ut, tincidunt massa.

### Other content blocks

> Vestibulum vitae orci quis ante viverra ultricies ut eget turpis. Sed eu
  lectus dapibus, eleifend nulla varius, lobortis turpis. In ac hendrerit nisl,
  sit amet laoreet nibh.
  ```
  var _extends = function(target) {
    for (var i = 1; i < arguments.length; i++) {
      var source = arguments[i];
      for (var key in source) {
        target[key] = source[key];
      }
    }
    return target;
  };
  ```

  > > Praesent at `:::js return target`, sodales nibh vel, tempor felis. Fusce
      vel lacinia lacus. Suspendisse rhoncus nunc non nisi iaculis ultrices.
      Donec consectetur mauris non neque imperdiet, eget volutpat libero.

## Lists

### Unordered lists

* Sed sagittis eleifend rutrum. Donec vitae suscipit est. Nullam tempus tellus
  non sem sollicitudin, quis rutrum leo facilisis. Nulla tempor lobortis orci,
  at elementum urna sodales vitae. In in vehicula nulla, quis ornare libero.

    * Duis mollis est eget nibh volutpat, fermentum aliquet dui mollis.
    * Nam vulputate tincidunt fringilla.
    * Nullam dignissim ultrices urna non auctor.

* Aliquam metus eros, pretium sed nulla venenatis, faucibus auctor ex. Proin ut
  eros sed sapien ullamcorper consequat. Nunc ligula ante, fringilla at aliquam
  ac, aliquet sed mauris.

* Nulla et rhoncus turpis. Mauris ultricies elementum leo. Duis efficitur
  accumsan nibh eu mattis. Vivamus tempus velit eros, porttitor placerat nibh
  lacinia sed. Aenean in finibus diam.

### Ordered lists

1. Integer vehicula feugiat magna, a mollis tellus. Nam mollis ex ante, quis
  elementum eros tempor rutrum. Aenean efficitur lobortis lacinia. Nulla
  consectetur feugiat sodales.

2. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur
  ridiculus mus. Aliquam ornare feugiat quam et egestas. Nunc id erat et quam
  pellentesque lacinia eu vel odio.

    1. Vivamus venenatis porttitor tortor sit amet rutrum. Pellentesque aliquet
      quam enim, eu volutpat urna rutrum a. Nam vehicula nunc mauris, a
      ultricies libero efficitur sed.

        1. Mauris dictum mi lacus
        2. Ut sit amet placerat ante
        3. Suspendisse ac eros arcu

    2. Morbi eget dapibus felis. Vivamus venenatis porttitor tortor sit amet
      rutrum. Pellentesque aliquet quam enim, eu volutpat urna rutrum a. Sed
      aliquet, neque at rutrum mollis, neque nisi tincidunt nibh.

    3. Pellentesque eget `:::js var _extends` ornare tellus, ut gravida mi.
    ```
    var _extends = function(target) {
      for (var i = 1; i < arguments.length; i++) {
        var source = arguments[i];
        for (var key in source) {
          target[key] = source[key];
        }
      }
      return target;
    };
    ```

3. Vivamus id mi enim. Integer id turpis sapien. Ut condimentum lobortis
  sagittis. Aliquam purus tellus, faucibus eget urna at, iaculis venenatis
  nulla. Vivamus a pharetra leo.

### Definition lists

**Not supported in commonmark, but you can use a rst definition list inside a
fenced eval_rst block.**

```eval_rst
Lorem ipsum dolor sit amet
   Sed sagittis eleifend rutrum. Donec vitae suscipit est. Nullam tempus
   tellus non sem sollicitudin, quis rutrum leo facilisis. Nulla tempor
   lobortis orci, at elementum urna sodales vitae. In in vehicula nulla.

   Duis mollis est eget nibh volutpat, fermentum aliquet dui mollis. Nam
   vulputate tincidunt fringilla. Nullam dignissim ultrices urna non
   auctor.

Cras arcu libero
   Aliquam metus eros, pretium sed nulla venenatis, faucibus auctor ex.
   Proin ut eros sed sapien ullamcorper consequat. Nunc ligula ante,
   fringilla at aliquam ac, aliquet sed mauris.
```

## Code blocks

### Inline

Morbi eget `dapibus felis`. Vivamus *`venenatis porttitor`* tortor sit amet
rutrum. Class aptent taciti sociosqu ad litora torquent per conubia nostra,
per inceptos himenaeos. [`Pellentesque aliquet quam enim`](#), eu volutpat urna
rutrum a.

Nam vehicula nunc `:::js return target` mauris, a ultricies libero efficitur
sed. Sed molestie imperdiet consectetur. Vivamus a pharetra leo. Pellentesque
eget ornare tellus, ut gravida mi. Fusce vel lacinia lacus.

### Listing

    var _extends = function(target) {
      for (var i = 1; i < arguments.length; i++) {
        var source = arguments[i];
        for (var key in source) {
          target[key] = source[key];
        }
      }
      return target;
    };

## Horizontal rules

Aenean in finibus diam. Duis mollis est eget nibh volutpat, fermentum aliquet
dui mollis. Nam vulputate tincidunt fringilla. Nullam dignissim ultrices urna
non auctor.

***

Integer vehicula feugiat magna, a mollis tellus. Nam mollis ex ante, quis
elementum eros tempor rutrum. Aenean efficitur lobortis lacinia. Nulla
consectetur feugiat sodales.

## Data tables

**Note**: Markdown table syntax requires ``sphinx_markdown_tables``

| Sollicitudo / Pellentesi | consectetur | adipiscing | elit    | arcu | sed |
| ------------------------ | ----------- | ---------- | ------- | ---- | --- |
| Vivamus a pharetra       | yes         | yes        | yes     | yes  | yes |
| Ornare viverra ex        | yes         | yes        | yes     | yes  | yes |
| Mauris a ullamcorper     | yes         | yes        | partial | yes  | yes |
| Nullam urna elit         | yes         | yes        | yes     | yes  | yes |
| Malesuada eget finibus   | yes         | yes        | yes     | yes  | yes |
| Ullamcorper              | yes         | yes        | yes     | yes  | yes |
| Vestibulum sodales       | yes         | -          | yes     | -    | yes |
| Pulvinar nisl            | yes         | yes        | yes     | -    | -   |
| Pharetra aliquet est     | yes         | yes        | yes     | yes  | yes |
| Sed suscipit             | yes         | yes        | yes     | yes  | yes |
| Orci non pretium         | yes         | partial    | -       | -    | -   |

Sed sagittis eleifend rutrum. Donec vitae suscipit est. Nullam tempus tellus
non sem sollicitudin, quis rutrum leo facilisis. Nulla tempor lobortis orci,
at elementum urna sodales vitae. In in vehicula nulla, quis ornare libero.

| Left       | Center   | Right   |
| :--------- | :------: | ------: |
| Lorem      | *dolor*  | `amet`  |
| [ipsum](#) | **sit**  |         |

Vestibulum vitae orci quis ante viverra ultricies ut eget turpis. Sed eu
lectus dapibus, eleifend nulla varius, lobortis turpis. In ac hendrerit nisl,
sit amet laoreet nibh.

<table>
  <colgroup>
    <col width="30%">
    <col width="70%">
  </colgroup>
  <thead>
    <tr class="header">
      <th>Table</th>
      <th>with colgroups (Pandoc)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Lorem</td>
      <td>ipsum dolor sit amet.</td>
    </tr>
    <tr>
      <td>Sed sagittis</td>
      <td>eleifend rutrum. Donec vitae suscipit est.</td>
    </tr>
  </tbody>
</table>