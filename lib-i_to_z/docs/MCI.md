<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.0//EN" "http://www.w3.org/TR/REC-html40/strict.dtd">

<html><head><title>MCI Library v1.0</title><style>/*
   IMPORTANT: If you're editing this file in the output directory of one of
   your projects, your changes will be overwritten the next time you run
   Natural Docs.  Instead, copy this file to your project directory, make your
   changes, and you can use it with -s.  Even better would be to make a CSS
   file in your project directory with only your changes, which you can then
   use with -s [original style] [your changes].

   On the other hand, if you're editing this file in the Natural Docs styles
   directory, the changes will automatically be applied to all your projects
   that use this style the next time Natural Docs is run on them.

   This file is part of Natural Docs, which is Copyright (C) 2003-2008 Greg Valure
   Natural Docs is licensed under the GPL
*/

body {
	font-family: Verdana, Arial, Helvetica, sans-serif, "MS sans serif";
    color: #000000;
    margin: 0; padding: 0;
    }

.ContentPage,
.IndexPage,
.FramedMenuPage {
    background-color: #E8E8E8;
    }
.FramedContentPage,
.FramedIndexPage,
.FramedSearchResultsPage,
.PopupSearchResultsPage {
    background-color: #FFFFFF;
    }


a:link,
a:visited { color: #900000; text-decoration: none }
a:hover { color: #900000; text-decoration: underline }
a:active { color: #FF0000; text-decoration: underline }

td {
    vertical-align: top }

img { border: 0;  }


/*
    Comment out this line to use web-style paragraphs (blank line between
    paragraphs, no indent) instead of print-style paragraphs (no blank line,
    indented.)
*/
p {
    text-indent: 0ex; margin-top: 2px; }


/*  Opera doesn't break with just wbr, but will if you add this.  */
.Opera wbr:after {
	content: "\00200B";
	}

/*  Blockquotes are used as containers for things that may need to scroll.  */
blockquote {
    padding: 0;
    margin: 0;
    overflow: auto;
    }


.Firefox1 blockquote {
    padding-bottom: .5em;
    }

/*  Turn off scrolling when printing.  */
@media print {
    blockquote {
        overflow: visible;
        }
    .IE blockquote {
        width: auto;
        }
    }



#Menu {
    font-size: 9pt;
    padding: 10px 0 0 0;
    }
.ContentPage #Menu,
.IndexPage #Menu {
    position: absolute;
    top: 0;
    left: 0;
    width: 31ex;
    overflow: hidden;
    }
.ContentPage .Firefox #Menu,
.IndexPage .Firefox #Menu {
    width: 27ex;
    }


    .MTitle {
        font-size: 16pt; font-weight: bold; font-variant: small-caps;
        text-align: center;
        padding: 5px 10px 15px 10px;
        border-bottom: 1px dotted #000000;
        margin-bottom: 15px }
    
    .MSubTitle {
        font-size: 9pt; font-weight: normal; font-variant: normal;
        margin-top: 1ex; margin-bottom: 5px }


    .MEntry a:link,
    .MEntry a:hover,
    .MEntry a:visited { color: #606060; margin-right: 0 }
    .MEntry a:active { color: #A00000; margin-right: 0 }


    .MGroup {
        font-variant: small-caps; font-weight: bold;
        margin: 1em 0 1em 10px;
        }
    
    .MGroupContent {
        font-variant: normal; font-weight: normal }
    
    .MGroup a:link,
    .MGroup a:hover,
    .MGroup a:visited { color: #545454; margin-right: 10px }
    .MGroup a:active { color: #A00000; margin-right: 10px }


    .MFile,
    .MText,
    .MLink,
    .MIndex {
        padding: 1px 17px 2px 10px;
        margin: .25em 0 .25em 0;
        }
    
    .MText {
        font-size: 8pt; font-style: italic }
    
    .MLink {
        font-style: italic }
    
    #MSelected {
        color: #000000; background-color: #FFFFFF;
        /*  Replace padding with border.  */
        padding: 0 10px 0 10px;
        border-width: 1px 2px 2px 0; border-style: solid; border-color: #000000;
        margin-right: 5px;
        }
    
    /*  Close off the left side when its in a group.  */
    .MGroup #MSelected {
        padding-left: 9px; border-left-width: 1px }
    
    /*  A treat for Mozilla users.  Blatantly non-standard.  Will be replaced with CSS 3 attributes when finalized/supported.  */
    .Firefox #MSelected {
        -moz-border-radius-topright: 10px;
        -moz-border-radius-bottomright: 10px }
    .Firefox .MGroup #MSelected {
        -moz-border-radius-topleft: 10px;
        -moz-border-radius-bottomleft: 10px }


    #MSearchPanel {
        padding: 0px 6px;
        margin: .25em 0;
        }


    #MSearchField {
        font: italic 9pt Verdana, sans-serif;
        color: #606060;
        background-color: #E8E8E8;
        border: none;
        padding: 2px 4px;
        width: 100%;
        }
    /* Only Opera gets it right. */
    .Firefox #MSearchField,
    .IE #MSearchField,
    .Safari #MSearchField {
        width: 94%;
        }
    .Opera9 #MSearchField,
    .Konqueror #MSearchField {
        width: 97%;
        }
    .FramedMenuPage .Firefox #MSearchField,
    .FramedMenuPage .Safari #MSearchField,
    .FramedMenuPage .Konqueror #MSearchField {
        width: 98%;
        }
    
    /* Firefox doesn't do this right in frames without #MSearchPanel added on.
        It's presence doesn't hurt anything other browsers. */
    #MSearchPanel.MSearchPanelInactive:hover #MSearchField {
        background-color: #FFFFFF;
        border: 1px solid #C0C0C0;
        padding: 1px 3px;
        }
    .MSearchPanelActive #MSearchField {
        background-color: #FFFFFF;
        border: 1px solid #C0C0C0;
        font-style: normal;
        padding: 1px 3px;
        }
    
    #MSearchType {
        visibility: hidden;
        font: 8pt Verdana, sans-serif;
        width: 98%;
        padding: 0;
        border: 1px solid #C0C0C0;
        }
    .MSearchPanelActive #MSearchType,
    /*  As mentioned above, Firefox doesn't do this right in frames without #MSearchPanel added on. */
    #MSearchPanel.MSearchPanelInactive:hover #MSearchType,
    #MSearchType:focus {
        visibility: visible;
        color: #606060;
        }
    #MSearchType option#MSearchEverything {
        font-weight: bold;
        }
    
    .Opera8 .MSearchPanelInactive:hover,
    .Opera8 .MSearchPanelActive {
        margin-left: -1px;
        }


    iframe#MSearchResults {
        width: 60ex;
        height: 15em;
        }
    #MSearchResultsWindow {
        display: none;
        position: absolute;
        left: 0; top: 0;
        border: 1px solid #000000;
        background-color: #E8E8E8;
        }
    #MSearchResultsWindowClose {
        font-weight: bold;
        font-size: 8pt;
        display: block;
        padding: 2px 5px;
        }
    #MSearchResultsWindowClose:link,
    #MSearchResultsWindowClose:visited {
        color: #000000;
        text-decoration: none;
        }
    #MSearchResultsWindowClose:active,
    #MSearchResultsWindowClose:hover {
        color: #800000;
        text-decoration: none;
        background-color: #F4F4F4;
        }




#Content {
    padding-bottom: 15px;
    }

.ContentPage #Content {
    border-width: 0 0 1px 1px;
    border-style: solid;
    border-color: #000000;
    background-color: #FFFFFF;
    font-size: 9pt;  /* To make 31ex match the menu's 31ex. */
    
    }
.ContentPage .Firefox #Content {
    margin-left: 27ex;
    }



    .CTopic {
        font-size: 10pt;
        margin-bottom: 3em;
        }


    .CTitle {
        font-size: 12pt; font-weight: bold;
        border-width: 0 0 1px 0; border-style: solid; border-color: #A0A0A0;
        margin: 0 15px .5em 15px }
    
    .CGroup .CTitle {
        font-size: 16pt; font-variant: small-caps;
        padding-left: 15px; padding-right: 15px;
        border-width: 0 0 2px 0; border-color: #000000;
        margin-left: 0; margin-right: 0 }
    
    .CClass .CTitle,
    .CInterface .CTitle,
    .CDatabase .CTitle,
    .CDatabaseTable .CTitle,
    .CSection .CTitle {
        font-size: 18pt;
        color: #FFFFFF; background-color: #A0A0A0;
        padding: 10px 15px 10px 15px;
        border-width: 2px 0; border-color: #000000;
        margin-left: 0; margin-right: 0 }
    
    #MainTopic .CTitle {
        font-size: 20pt;
        color: #FFFFFF; background-color: #7070C0;
        padding: 10px 15px 10px 15px;
        border-width: 0 0 3px 0; border-color: #000000;
        margin-left: 0; margin-right: 0 }
    
    .CBody {
        margin-left: 15px; margin-right: 15px }


    .CToolTip {
        position: absolute; visibility: hidden;
        left: 0; top: 0;
        background-color: #FFFFE0;
        padding: 5px;
        border-width: 1px 2px 2px 1px; border-style: solid; border-color: #000000;
        font-size: 8pt;
        }
    
    .Opera .CToolTip {
        max-width: 98%;
        }
    
    /*  Scrollbars would be useless.  */
    .CToolTip blockquote {
        overflow: hidden;
        }
    .IE6 .CToolTip blockquote {
        overflow: visible;
        }
    
    .CHeading {
        font-weight: bold; font-size: 10pt;
        margin: 1.5em 0 .5em 0;
        }
    
    .CBody pre {
        font: 9pt "Courier New", Courier, monospace;
        margin: 1em 0;
        }
    
    .CBody ul {
        /*  I don't know why CBody's margin doesn't apply, but it's consistent across browsers so whatever.
             Reapply it here as padding.  */
        padding-left: 15px; padding-right: 15px;
        margin: .5em 5ex .5em 5ex;
        }
    
    .CDescriptionList {
        margin: .5em 5ex 0 5ex }
    
    .CDLEntry {
            font: 10pt "Courier New", Courier, monospace; color: #808080;
            padding-bottom: .25em;
            white-space: nowrap }
    
    CDLDescription {
            font-size: 10pt;  /*  For browsers that don't inherit correctly, like Opera 5.  */
            padding-bottom: .5em; padding-left: 5ex }


    .CTopic img {
        text-align: center;
        display: block;
        margin: 1em auto;
        }
    .CImageCaption {
        font-variant: small-caps;
        font-size: 8pt;
        color: #808080;
        text-align: center;
        position: relative;
        top: 1em;
        }
    
    .CImageLink {
        color: #808080;
        font-style: italic;
        }
    a.CImageLink:link,
    a.CImageLink:visited,
    a.CImageLink:hover { color: #808080 }





.Prototype {
    font: 10pt "Courier New", Courier, monospace;
    padding: 5px 3ex;
    border-width: 1px; border-style: solid;
    margin: 0 5ex 1.5em 5ex;
    }

    .Prototype td {
        font-size: 10pt;
        }
    
    .PDefaultValue,
    .PDefaultValuePrefix,
    .PTypePrefix {
        color: #8F8F8F;
        }
    .PTypePrefix {
        text-align: right;
        }
    .PAfterParameters {
        vertical-align: bottom;
        }
    
    .IE .Prototype table {
        padding: 0;
        }
    
    .CFunction .Prototype {
        background-color: #F4F4F4; border-color: #D0D0D0 }
    .CProperty .Prototype {
        background-color: #F4F4FF; border-color: #C0C0E8 }
    .CVariable .Prototype {
        background-color: #FFFFF0; border-color: #E0E0A0 }
    
    .CClass .Prototype {
        border-width: 1px 2px 2px 1px; border-style: solid; border-color: #A0A0A0;
        background-color: #F4F4F4;
        }
    .CInterface .Prototype {
        border-width: 1px 2px 2px 1px; border-style: solid; border-color: #A0A0D0;
        background-color: #F4F4FF;
        }
    
    .CDatabaseIndex .Prototype,
    .CConstant .Prototype {
        background-color: #D0D0D0; border-color: #000000 }
    .CType .Prototype,
    .CEnumeration .Prototype {
        background-color: #FAF0F0; border-color: #E0B0B0;
        }
    .CDatabaseTrigger .Prototype,
    .CEvent .Prototype,
    .CDelegate .Prototype {
        background-color: #F0FCF0; border-color: #B8E4B8 }
    
    .CToolTip .Prototype {
        margin: 0 0 .5em 0;
        white-space: nowrap;
        }





.Summary {
    margin: 1.5em 5ex 0 5ex }

    .STitle {
        font-size: 12pt; font-weight: bold;
        margin-bottom: .5em }


    .SBorder {
        background-color: #FFFFF0;
        padding: 15px;
        border: 1px solid #C0C060 }
    
    /* In a frame IE 6 will make them too long unless you set the width to 100%.  Without frames it will be correct without a width
        or slightly too long (but not enough to scroll) with a width.  This arbitrary weirdness simply astounds me.  IE 7 has the same
        problem with frames, haven't tested it without.  */
    .FramedContentPage .IE .SBorder {
        width: 100% }
    
    /*  A treat for Mozilla users.  Blatantly non-standard.  Will be replaced with CSS 3 attributes when finalized/supported.  */
    .Firefox .SBorder {
        -moz-border-radius: 20px }


    .STable {
        font-size: 9pt; width: 100% }
    
    .SEntry {
        width: 30% }
    .SDescription {
        width: 70% }


    .SMarked {
        background-color: #F8F8D8 }
    
    .SDescription { padding-left: 2ex }
    .SIndent1 .SEntry { padding-left: 1.5ex }   .SIndent1 .SDescription { padding-left: 3.5ex }
    .SIndent2 .SEntry { padding-left: 3.0ex }   .SIndent2 .SDescription { padding-left: 5.0ex }
    .SIndent3 .SEntry { padding-left: 4.5ex }   .SIndent3 .SDescription { padding-left: 6.5ex }
    .SIndent4 .SEntry { padding-left: 6.0ex }   .SIndent4 .SDescription { padding-left: 8.0ex }
    .SIndent5 .SEntry { padding-left: 7.5ex }   .SIndent5 .SDescription { padding-left: 9.5ex }
    
    .SDescription a { color: #800000}
    .SDescription a:active { color: #A00000 }
    
    .SGroup td {
        padding-top: .5em; padding-bottom: .25em }
    
    .SGroup .SEntry {
        font-weight: bold; font-variant: small-caps }
    
    .SGroup .SEntry a { color: #800000 }
    .SGroup .SEntry a:active { color: #F00000 }


    .SMain td,
    .SClass td,
    .SDatabase td,
    .SDatabaseTable td,
    .SSection td {
        font-size: 10pt;
        padding-bottom: .25em }
    
    .SClass td,
    .SDatabase td,
    .SDatabaseTable td,
    .SSection td {
        padding-top: 1em }
    
    .SMain .SEntry,
    .SClass .SEntry,
    .SDatabase .SEntry,
    .SDatabaseTable .SEntry,
    .SSection .SEntry {
        font-weight: bold;
        }
    
    .SMain .SEntry a,
    .SClass .SEntry a,
    .SDatabase .SEntry a,
    .SDatabaseTable .SEntry a,
    .SSection .SEntry a { color: #000000 }
    
    .SMain .SEntry a:active,
    .SClass .SEntry a:active,
    .SDatabase .SEntry a:active,
    .SDatabaseTable .SEntry a:active,
    .SSection .SEntry a:active { color: #A00000 }





.ClassHierarchy {
    margin: 0 15px 1em 15px }

    .CHEntry {
        border-width: 1px 2px 2px 1px; border-style: solid; border-color: #A0A0A0;
        margin-bottom: 3px;
        padding: 2px 2ex;
        font-size: 10pt;
        background-color: #F4F4F4; color: #606060;
        }
    
    .Firefox .CHEntry {
        -moz-border-radius: 4px;
        }
    
    .CHCurrent .CHEntry {
        font-weight: bold;
        border-color: #000000;
        color: #000000;
        }
    
    .CHChildNote .CHEntry {
        font-style: italic;
        font-size: 8pt;
        }
    
    .CHIndent {
        margin-left: 3ex;
        }
    
    .CHEntry a:link,
    .CHEntry a:visited,
    .CHEntry a:hover {
        color: #606060;
        }
    .CHEntry a:active {
        color: #800000;
        }





#Index {
    background-color: #FFFFFF;
    }

/*  As opposed to .PopupSearchResultsPage #Index  */
.IndexPage #Index,
.FramedIndexPage #Index,
.FramedSearchResultsPage #Index {
    padding: 15px;
    }

.IndexPage #Index {
    border-width: 0 0 1px 1px;
    border-style: solid;
    border-color: #000000;
    font-size: 9pt;  /* To make 27ex match the menu's 27ex. */
    margin-left: 27ex;
    }


    .IPageTitle {
        font-size: 20pt; font-weight: bold;
        color: #FFFFFF; background-color: #7070C0;
        padding: 10px 15px 10px 15px;
        border-width: 0 0 3px 0; border-color: #000000; border-style: solid;
        margin: -15px -15px 0 -15px }
    
    .FramedSearchResultsPage .IPageTitle {
        margin-bottom: 15px;
        }
    
    .INavigationBar {
        font-size: 10pt;
        text-align: center;
        background-color: #FFFFF0;
        padding: 5px;
        border-bottom: solid 1px black;
        margin: 0 -15px 15px -15px;
        }
    
    .INavigationBar a {
        font-weight: bold }
    
    .IHeading {
        font-size: 16pt; font-weight: bold;
        padding: 2.5em 0 .5em 0;
        text-align: center;
        width: 3.5ex;
        }
    #IFirstHeading {
        padding-top: 0;
        }
    
    .IEntry {
        font-size: 10pt;
        padding-left: 1ex;
        }
    .PopupSearchResultsPage .IEntry {
        font-size: 8pt;
        padding: 1px 5px;
        }
    .PopupSearchResultsPage .Opera9 .IEntry,
    .FramedSearchResultsPage .Opera9 .IEntry {
        text-align: left;
        }
    .FramedSearchResultsPage .IEntry {
        padding: 0;
        }
    
    .ISubIndex {
        padding-left: 3ex; padding-bottom: .5em }
    .PopupSearchResultsPage .ISubIndex {
        display: none;
        }


    /*  While it may cause some entries to look like links when they aren't, I found it's much easier to read the
         index if everything's the same color.  */
    .ISymbol {
        font-weight: bold; color: #900000  }
    
    .IndexPage .ISymbolPrefix,
    .FramedIndexPage .ISymbolPrefix {
        font-size: 10pt;
        text-align: right;
        color: #C47C7C;
        background-color: #F8F8F8;
        border-right: 3px solid #E0E0E0;
        border-left: 1px solid #E0E0E0;
        padding: 0 1px 0 2px;
        }
    .PopupSearchResultsPage .ISymbolPrefix,
    .FramedSearchResultsPage .ISymbolPrefix {
        color: #900000;
        }
    .PopupSearchResultsPage .ISymbolPrefix {
        font-size: 8pt;
        }
    
    .IndexPage #IFirstSymbolPrefix,
    .FramedIndexPage #IFirstSymbolPrefix {
        border-top: 1px solid #E0E0E0;
        }
    .IndexPage #ILastSymbolPrefix,
    .FramedIndexPage #ILastSymbolPrefix {
        border-bottom: 1px solid #E0E0E0;
        }
    .IndexPage #IOnlySymbolPrefix,
    .FramedIndexPage #IOnlySymbolPrefix {
        border-top: 1px solid #E0E0E0;
        border-bottom: 1px solid #E0E0E0;
        }
    
    a.IParent,
    a.IFile {
        display: block;
        }
    
    .PopupSearchResultsPage .SRStatus {
        padding: 2px 5px;
        font-size: 8pt;
        font-style: italic;
        }
    .FramedSearchResultsPage .SRStatus {
        font-size: 10pt;
        font-style: italic;
        }
    
    .SRResult {
        display: none;
        }



#Footer {
    font-size: 8pt;
    color: #989898;
    text-align: right;
    }

#Footer p {
    text-indent: 0;
    margin-bottom: .5em;
    }

.ContentPage #Footer,
.IndexPage #Footer {
    text-align: right;
    margin: 2px;
    }

.FramedMenuPage #Footer {
    text-align: center;
    margin: 5em 10px 10px 10px;
    padding-top: 1em;
    border-top: 1px solid #C8C8C8;
    }

    #Footer a:link,
    #Footer a:hover,
    #Footer a:visited { color: #989898 }
    #Footer a:active { color: #A00000 }


#MainTopic .CTitle {					/* Title: */
  font-size: 20pt;
  font-weight: bold; /* Bold looks better against dark background. */
  font-family: Arial, Helvetica, sans-serif, "MS sans serif"; 
  background-color: #405871;
  color: #FFFFFF;
  margin: 0 0 0.5em 0;
  padding: 10px 15px 10px 15px;
}


.SBorder,.SEntry, .SDescription {				/* Summary index */
  background-color: #F2F2F2;
  padding: 5px;
  border: 1px solid #E0E0E0 }
.SBorder{ padding: 1px; }


.CTitle {							/* Function */
  background-color: #FFFFAA;
  margin: 1 1 1 1;
  padding: 12px 0 12px 4px;
  font-size: 12pt; font-weight: bold;
  border-width: 3px 0px 0px 0; border-style: solid; border-color: #A0A0A0;
}


h4 {							/* topics.. (parameters, returns, example..) */
  font-size: 111%;  font-weight: bold;
  background-color:#E6E6E6;
  margin: 1.0em 0 0.5em 0;
  padding: 0.1em 0 0.1em 0.2em;
}


.CDescriptionList, .CDLEntry, .CDLDescription {			/* parameter table */
  width: 100%;
  margin: 1em 0ex 0 0ex;
  border-width: 1px 1px 1px 1px; border-style: solid; border-color: #C0C0C0;
}
.CDLEntry, .CDLDescription { margin: 0 0 0em 0;  text-indent: 0px;  padding-left: 1ex; padding-bottom: .5em; padding-top: .5em; }
.CDLEntry { width: 15%; font: 10pt "Courier New", Courier, monospace; }

/*  Blockquotes are used as containers for things that may need to scroll.  */
blockquote {
    padding: 20;
        padding-left: 9px; border-left-width: 1px;
    margin: 0;
    overflow: auto;
    background-color: #F3F3FF;			/* example bg color..*/
        border-width: 0px 0px 0px 0px; border-style: solid; border-color: #838B8B;
    }

/* .ContentPage #Content { margin-left: 0ex; }   */


a        {text-decoration: none;}
a:link   {text-decoration: none; color: #0000AA;}
a:visited{text-decoration: none; color: #AA00AA;}
a:active {text-decoration: none; color: #0000AA;}
a:hover  {text-decoration: underline; color: #6666CC;}</style><script language=JavaScript src="../javascript/main.js"></script><script language=JavaScript src="../javascript/searchdata.js"></script></head><body class="ContentPage" onLoad="NDOnLoad()"><script language=JavaScript><!--
if (browserType) {document.write("<div class=" + browserType + ">");if (browserVer) {document.write("<div class=" + browserVer + ">"); }}// --></script>

<!--  Generated by Natural Docs, version 1.4 -->
<!--  http://www.naturaldocs.org  -->

<!-- saved from url=(0026)http://www.naturaldocs.org -->




<div id=Content><div class="CSection"><div class=CTopic id=MainTopic><h1 class=CTitle><a name="MCI_Library_v1.0"></a>MCI Library v1.0</h1><div class=CBody><!--START_ND_SUMMARY--><div class=Summary><div class=STitle>Summary</div><div class=SBorder><table border=0 cellspacing=0 cellpadding=0 class=STable><tr class="SMain"><td class=SEntry><a href="#MCI_Library_v1.0" >MCI Library v1.0</a></td><td class=SDescription></td></tr><tr class="SGroup SIndent1"><td class=SEntry><a href="#Overview" >Overview</a></td><td class=SDescription>This library gives the AutoHotkey developer access to the the Media Control Interface (MCI) which provides standard commands for playing/controlling multimedia devices.</td></tr><tr class="SGroup SIndent1"><td class=SEntry><a href="#Notes" >Notes</a></td><td class=SDescription></td></tr><tr class="SGroup SIndent1"><td class=SEntry><a href="#Links" >Links</a></td><td class=SDescription>MCI Reference Guide</td></tr><tr class="SGroup SIndent1"><td class=SEntry><a href="#Credit" >Credit</a></td><td class=SDescription>The MCI library is an offshoot of the Sound_* and Media_* libraries provided by <b>Fincs</b>.</td></tr><tr class="SGroup SIndent1"><td class=SEntry><a href="#Functions" >Functions</a></td><td class=SDescription></td></tr><tr class="SFunction SIndent2 SMarked"><td class=SEntry><a href="#MCI_Close" id=link1 onMouseOver="ShowTip(event, 'tt1', 'link1')" onMouseOut="HideTip('tt1')">MCI_Close</a></td><td class=SDescription>Closes the device and any associated resources.</td></tr><tr class="SFunction SIndent2"><td class=SEntry><a href="#MCI_CurrentTrack" id=link2 onMouseOver="ShowTip(event, 'tt2', 'link2')" onMouseOut="HideTip('tt2')">MCI_CurrentTrack</a></td><td class=SDescription>Identifies the current track.</td></tr><tr class="SFunction SIndent2 SMarked"><td class=SEntry><a href="#MCI_DeviceType" id=link3 onMouseOver="ShowTip(event, 'tt3', 'link3')" onMouseOut="HideTip('tt3')">MCI_DeviceType</a></td><td class=SDescription>Identifies the device type name.</td></tr><tr class="SFunction SIndent2"><td class=SEntry><a href="#MCI_Open" id=link4 onMouseOver="ShowTip(event, 'tt4', 'link4')" onMouseOut="HideTip('tt4')">MCI_Open</a></td><td class=SDescription>Opens an MCI device and loads the specified file.</td></tr><tr class="SFunction SIndent2 SMarked"><td class=SEntry><a href="#MCI_OpenCDAudio" id=link5 onMouseOver="ShowTip(event, 'tt5', 'link5')" onMouseOut="HideTip('tt5')">MCI_OpenCDAudio</a></td><td class=SDescription>Opens a CDAudio device.</td></tr><tr class="SFunction SIndent2"><td class=SEntry><a href="#MCI_Length" id=link6 onMouseOver="ShowTip(event, 'tt6', 'link6')" onMouseOut="HideTip('tt6')">MCI_Length</a></td><td class=SDescription>Gets the total length of the media in the current time format.</td></tr><tr class="SFunction SIndent2 SMarked"><td class=SEntry><a href="#MCI_MediaIsPresent" id=link7 onMouseOver="ShowTip(event, 'tt7', 'link7')" onMouseOut="HideTip('tt7')">MCI_MediaIsPresent</a></td><td class=SDescription>Checks to see if media is present in the device.</td></tr><tr class="SFunction SIndent2"><td class=SEntry><a href="#MCI_Notify" id=link8 onMouseOver="ShowTip(event, 'tt8', 'link8')" onMouseOut="HideTip('tt8')">MCI_Notify</a></td><td class=SDescription>(Internal function. </td></tr><tr class="SFunction SIndent2 SMarked"><td class=SEntry><a href="#MCI_NumberOfTracks" id=link9 onMouseOver="ShowTip(event, 'tt9', 'link9')" onMouseOut="HideTip('tt9')">MCI_NumberOfTracks</a></td><td class=SDescription>Identifies the number of tracks on the media.</td></tr><tr class="SFunction SIndent2"><td class=SEntry><a href="#MCI_Pause" id=link10 onMouseOver="ShowTip(event, 'tt10', 'link10')" onMouseOut="HideTip('tt10')">MCI_Pause</a></td><td class=SDescription>Pauses playback or recording.</td></tr><tr class="SFunction SIndent2 SMarked"><td class=SEntry><a href="#MCI_Play" id=link11 onMouseOver="ShowTip(event, 'tt11', 'link11')" onMouseOut="HideTip('tt11')">MCI_Play</a></td><td class=SDescription>Starts playing a device.</td></tr><tr class="SFunction SIndent2"><td class=SEntry><a href="#MCI_Position" id=link12 onMouseOver="ShowTip(event, 'tt12', 'link12')" onMouseOut="HideTip('tt12')">MCI_Position</a></td><td class=SDescription>Identifies the current playback or recording position.</td></tr><tr class="SFunction SIndent2 SMarked"><td class=SEntry><a href="#MCI_Record" id=link13 onMouseOver="ShowTip(event, 'tt13', 'link13')" onMouseOut="HideTip('tt13')">MCI_Record</a></td><td class=SDescription>Starts recording.</td></tr><tr class="SFunction SIndent2"><td class=SEntry><a href="#MCI_Resume" id=link14 onMouseOver="ShowTip(event, 'tt14', 'link14')" onMouseOut="HideTip('tt14')">MCI_Resume</a></td><td class=SDescription>Resumes playback or recording after the device has been paused. </td></tr><tr class="SFunction SIndent2 SMarked"><td class=SEntry><a href="#MCI_Save" id=link15 onMouseOver="ShowTip(event, 'tt15', 'link15')" onMouseOut="HideTip('tt15')">MCI_Save</a></td><td class=SDescription>Saves an MCI file.</td></tr><tr class="SFunction SIndent2"><td class=SEntry><a href="#MCI_Seek" >MCI_Seek</a></td><td class=SDescription>Move to a specified position.</td></tr><tr class="SFunction SIndent2 SMarked"><td class=SEntry><a href="#MCI_SetBass" id=link16 onMouseOver="ShowTip(event, 'tt16', 'link16')" onMouseOut="HideTip('tt16')">MCI_SetBass</a></td><td class=SDescription>Sets the audio low frequency level.</td></tr><tr class="SFunction SIndent2"><td class=SEntry><a href="#MCI_SetTreble" id=link17 onMouseOver="ShowTip(event, 'tt17', 'link17')" onMouseOut="HideTip('tt17')">MCI_SetTreble</a></td><td class=SDescription>Sets the audio high-frequency level.</td></tr><tr class="SFunction SIndent2 SMarked"><td class=SEntry><a href="#MCI_SetVolume" id=link18 onMouseOver="ShowTip(event, 'tt18', 'link18')" onMouseOut="HideTip('tt18')">MCI_SetVolume</a></td><td class=SDescription>Sets the average audio volume for both audio channels. </td></tr><tr class="SFunction SIndent2"><td class=SEntry><a href="#MCI_Status" id=link19 onMouseOver="ShowTip(event, 'tt19', 'link19')" onMouseOut="HideTip('tt19')">MCI_Status</a></td><td class=SDescription>Identifies the current mode of the device.</td></tr><tr class="SFunction SIndent2 SMarked"><td class=SEntry><a href="#MCI_Stop" id=link20 onMouseOver="ShowTip(event, 'tt20', 'link20')" onMouseOut="HideTip('tt20')">MCI_Stop</a></td><td class=SDescription>Stops playback or recording.</td></tr><tr class="SFunction SIndent2"><td class=SEntry><a href="#MCI_TrackIsAudio" id=link21 onMouseOver="ShowTip(event, 'tt21', 'link21')" onMouseOut="HideTip('tt21')">MCI_TrackIsAudio</a></td><td class=SDescription>Determines if the specified track is an audio track.</td></tr><tr class="SFunction SIndent2 SMarked"><td class=SEntry><a href="#MCI_ToHHMMSS" id=link22 onMouseOver="ShowTip(event, 'tt22', 'link22')" onMouseOut="HideTip('tt22')">MCI_ToHHMMSS</a></td><td class=SDescription>Converts the specified number of milliseconds to hh:mm:ss format.</td></tr><tr class="SFunction SIndent2"><td class=SEntry><a href="#MCI_ToMilliseconds" id=link23 onMouseOver="ShowTip(event, 'tt23', 'link23')" onMouseOut="HideTip('tt23')">MCI_ToMilliseconds</a></td><td class=SDescription>Converts the specified hour, minute and second into a valid milliseconds timestamp.</td></tr><tr class="SFunction SIndent2 SMarked"><td class=SEntry><a href="#MCI_SendString" id=link24 onMouseOver="ShowTip(event, 'tt24', 'link24')" onMouseOut="HideTip('tt24')">MCI_SendString</a></td><td class=SDescription>This is the primary function that controls MCI operations. </td></tr></table></div></div><!--END_ND_SUMMARY--></div></div></div>

<div class="CGroup"><div class=CTopic><h3 class=CTitle><a name="Overview"></a>Overview</h3><div class=CBody><p>This library gives the AutoHotkey developer access to the the Media Control Interface (MCI) which provides standard commands for playing/controlling multimedia devices.</p></div></div></div>

<div class="CGroup"><div class=CTopic><h3 class=CTitle><a name="Notes"></a>Notes</h3><div class=CBody><h4 class=CHeading>Devices Referenced Within The Documentation</h4><blockquote><pre>Driver      Type            Description
------      ----            -----------
MCIAVI      avivideo
MCICDA      cdaudio         CD audio
            dat             Digital-audio tape player
            digitalvideo    Digital video in a window (not GDI-based)
            MPEGVideo       General-purpose media player
            other           Undefined MCI device
            overlay         Overlay device (analog video in a window)
            scanner         Image scanner
MCISEQ      sequencer       MIDI sequencer
            vcr             Video-cassette recorder or player
MCIPIONR    videodisc       Videodisc (Pioneer LaserDisc)
MCIWAVE     waveaudio       Audio device that plays digitized waveform files</pre></blockquote><h4 class=CHeading>MCI Installation</h4><p>To see a list of MCI devices that have been registered for the computer, go to the following registry locations...</p><blockquote><pre>Windows NT4/2000/XP/2003/Vista/etc.:

  16-bit:
    HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\MCI

  32-bit:
    HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\MCI32


Windows 95/98/ME:

    HKEY_LOCAL_MACHINE\System\CurrentControlSet\Control\MediaResources\MCI</pre></blockquote><p>To see a list of registered file extensions and the MCI device that has been assigned to each extension, go the following locations...</p><blockquote><pre>For Windows NT4/2000/XP/2003/Vista/etc., this information is stored in
the following registry location:

    HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\MCI Extensions

For Windows 95/98/ME, this information is stored in the %windir%\win.ini
file in the &quot;MCI Extensions&quot; section.</pre></blockquote><h4 class=CHeading>Debugging</h4><p><b>OutputDebug</b> statements in the core of some of the functions that only execute on condition are permanent and are provided to help the developer find and eliminate errors.</p></div></div></div>

<div class="CGroup"><div class=CTopic><h3 class=CTitle><a name="Links"></a>Links</h3><div class=CBody><p>MCI Reference Guide</p><ul><li><a href="http://msdn.microsoft.com/en-us/library/ms709461(VS.85).aspx" class=LURL target=_top>http://msdn.microsoft.com<wbr>/en-us<wbr>/library<wbr>/ms709461(VS.85).aspx</a></li></ul></div></div></div>

<div class="CGroup"><div class=CTopic><h3 class=CTitle><a name="Credit"></a>Credit</h3><div class=CBody><p>The MCI library is an offshoot of the Sound_* and Media_* libraries provided by <b>Fincs</b>.</p><ul><li><a href="http://www.autohotkey.com/forum/viewtopic.php?t=20666" class=LURL target=_top>http://www.autohotkey.com<wbr>/forum<wbr>/viewtopic.php?t=20666</a></li><li><a href="http://www.autohotkey.com/forum/viewtopic.php?t=22662" class=LURL target=_top>http://www.autohotkey.com<wbr>/forum<wbr>/viewtopic.php?t=22662</a></li></ul><p>Credit and thanks to <b>Fincs</b> for creating and enhancing  these libraries which are a conversion from the AutoIt &ldquo;Sound.au3&rdquo; standard library and to <b>RazerM</b> for providing the original &ldquo;Sound.au3&rdquo; library.</p><p>Notify idea and code from <b>Sean</b></p><ul><li><a href="http://www.autohotkey.com/forum/viewtopic.php?p=132331#132331" class=LURL target=_top>http://www.autohotkey.com<wbr>/forum<wbr>/viewtopic.php?p=132331#132331</a></li></ul><p>mciGetErrorString call from <b>PhiLho</b></p><ul><li><a href="http://www.autohotkey.com/forum/viewtopic.php?p=116011#116011" class=LURL target=_top>http://www.autohotkey.com<wbr>/forum<wbr>/viewtopic.php?p=116011#116011</a></li></ul></div></div></div>

<div class="CGroup"><div class=CTopic><h3 class=CTitle><a name="Functions"></a>Functions</h3></div></div>

<div class="CFunction"><div class=CTopic><h3 class=CTitle><a name="MCI_Close"></a>MCI_Close</h3><div class=CBody><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_Close(</td><td class=PParameter nowrap>p_lpszDeviceID</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote><h4 class=CHeading>Description</h4><p>Closes the device and any associated resources.</p><h4 class=CHeading>Parameters</h4><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>p_lpszDeviceID</td><td class=CDLDescription>Device name or alias.</td></tr></table><h4 class=CHeading>Returns</h4><p>The return code from the <a href="#MCI_SendString" class=LFunction id=link25 onMouseOver="ShowTip(event, 'tt24', 'link25')" onMouseOut="HideTip('tt24')">MCI_SendString</a> function which is 0 if the command completed successfully.</p><h4 class=CHeading>Remarks</h4><p>For most MCI devices, closing a device usually stops playback but not always.&nbsp;  If unsure of the device, consider stopping the device before closing it.</p></div></div></div>

<div class="CFunction"><div class=CTopic><h3 class=CTitle><a name="MCI_CurrentTrack"></a>MCI_CurrentTrack</h3><div class=CBody><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_CurrentTrack(</td><td class=PParameter nowrap>p_lpszDeviceID</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote><h4 class=CHeading>Description</h4><p>Identifies the current track.</p><h4 class=CHeading>Parameters</h4><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>p_lpszDeviceID</td><td class=CDLDescription>Device name or alias.</td></tr></table><h4 class=CHeading>Returns</h4><p>The current track.&nbsp; Note: The MCISEQ sequencer returns 1.</p></div></div></div>

<div class="CFunction"><div class=CTopic><h3 class=CTitle><a name="MCI_DeviceType"></a>MCI_DeviceType</h3><div class=CBody><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_DeviceType(</td><td class=PParameter nowrap>p_lpszDeviceID</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote><h4 class=CHeading>Description</h4><p>Identifies the device type name.</p><h4 class=CHeading>Parameters</h4><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>p_lpszDeviceID</td><td class=CDLDescription>Device name or alias.</td></tr></table><h4 class=CHeading>Returns</h4><p>A device type name, which can be one of the following...</p><blockquote><pre>cdaudio
dat
digitalvideo
other
overlay
scanner
sequencer
vcr
videodisc
waveaudio</pre></blockquote></div></div></div>

<div class="CFunction"><div class=CTopic><h3 class=CTitle><a name="MCI_Open"></a>MCI_Open</h3><div class=CBody><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_Open(</td><td class=PParameter nowrap>p_MediaFile,</td><td class=PDefaultValuePrefix>&nbsp;&nbsp;</td><td class=PDefaultValue width=100%></td></tr><tr><td></td><td class=PParameter nowrap>p_Alias</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>&quot;&quot;,</td></tr><tr><td></td><td class=PParameter nowrap>p_Flags</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>&quot;&quot;</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote><h4 class=CHeading>Description</h4><p>Opens an MCI device and loads the specified file.</p><h4 class=CHeading>Parameters</h4><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>p_MediaFile</td><td class=CDLDescription>A multimedia file.</td></tr><tr><td class=CDLEntry>p_Alias</td><td class=CDLDescription>Alias.&nbsp; A name such as media1.&nbsp; [Optional] If blank (the default), an alias will automatically be generated.</td></tr><tr><td class=CDLEntry>p_Flags</td><td class=CDLDescription>Flags that determine how the device is opened.&nbsp; [Optional]</td></tr></table><h4 class=CHeading>Flag Notes</h4><p>Some commonly used flags include...</p><blockquote><pre>type {device_type}
sharable</pre></blockquote><p>If more than one flag is used, separate each flag/value with a space.&nbsp; For example:</p><blockquote><pre>type MPEGVideo sharable</pre></blockquote><p>Additional notes...</p><ul><li>The &ldquo;wait&rdquo; flag is automatically added to the end of the command string.&nbsp; This flag directs the device to complete the &ldquo;open&rdquo; request before returning.</li><li>Use the &ldquo;shareable&rdquo; flag with care.&nbsp;  Per msdn, the &ldquo;shareable&rdquo; flag &ldquo;initializes the device or file as shareable.&nbsp; Subsequent attempts to open the device or file fail unless you specify &ldquo;shareable&rdquo; in both the original and subsequent open commands.&nbsp;  MCI returns an invalid device error if the device is already open and not shareable.&nbsp;  The MCISEQ sequencer and MCIWAVE devices do not support shared files.&rdquo;</li><li>By default, the MCI device that is opened is determined by the file&rsquo;s extension.&nbsp;  The &ldquo;type&rdquo; flag can be used to  1) override the default device that is registered for the file extension or to  2) open a media file with a file extension that is not registered as a MCI file extension.&nbsp;  See the <a href="#Notes" class=LGroup >Notes</a> section for more information.</li><li>For a complete list of flags and descriptions for the &ldquo;open&rdquo; command string, see the &ldquo;MCI Reference Guide&rdquo; in the <a href="#Links" class=LGroup id=link26 onMouseOver="ShowTip(event, 'tt25', 'link26')" onMouseOut="HideTip('tt25')">Links</a> section.</li></ul><h4 class=CHeading>Returns</h4><p>The multimedia handle (alias) or 0 (FALSE) to indicate failure.&nbsp;  Failure will occur with any of the following conditions:</p><ul><li>The media file does not exist.</li><li>The media file&rsquo;s extension is not a regisitered MCI extension.&nbsp; Note: This test is only performed if the &ldquo;type&rdquo; flag is not specified.</li><li>Non-zero return code from the <a href="#MCI_SendString" class=LFunction id=link27 onMouseOver="ShowTip(event, 'tt24', 'link27')" onMouseOut="HideTip('tt24')">MCI_SendString</a> function.</li></ul><h4 class=CHeading>Remarks</h4><ul><li>Use the <a href="#MCI_OpenCDAudio" class=LFunction id=link28 onMouseOver="ShowTip(event, 'tt5', 'link28')" onMouseOut="HideTip('tt5')">MCI_OpenCDAudio</a> function to open a CDAudio device.</li><li>After the device has been successfully opened, the time format is set to milliseconds which it will remain in effect until it is manually set to another value or until the device is closed.</li></ul></div></div></div>

<div class="CFunction"><div class=CTopic><h3 class=CTitle><a name="MCI_OpenCDAudio"></a>MCI_OpenCDAudio</h3><div class=CBody><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_OpenCDAudio(</td><td class=PParameter nowrap>p_Drive</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>&quot;&quot;,</td></tr><tr><td></td><td class=PParameter nowrap>p_Alias</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>&quot;&quot;,</td></tr><tr><td></td><td class=PParameter nowrap>p_CheckForMedia</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>True</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote><h4 class=CHeading>Description</h4><p>Opens a CDAudio device.</p><h4 class=CHeading>Parameters</h4><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>p_Drive</td><td class=CDLDescription>CDROM drive letter.&nbsp; [Optional] If blank (the default), the first CDROM drive found is used.</td></tr><tr><td class=CDLEntry>p_Alias</td><td class=CDLDescription>Alias.&nbsp;  A name such as media1.&nbsp; [Optional] If blank (the default), an alias will automatically be generated.</td></tr><tr><td class=CDLEntry>p_CheckForMedia</td><td class=CDLDescription>Check for media.&nbsp; [Optional] The default is TRUE.</td></tr></table><h4 class=CHeading>Returns</h4><p>The multimedia handle (alias) or 0 to indicate failure.&nbsp;  Failure will occur with any of the following conditions:</p><ul><li>The computer does not have a CDROM drive.</li><li>The specified drive is not CDROM drive.</li><li>Non-zero return code from the <a href="#MCI_SendString" class=LFunction id=link29 onMouseOver="ShowTip(event, 'tt24', 'link29')" onMouseOut="HideTip('tt24')">MCI_SendString</a> function.</li></ul><p>If p_CheckForMedia is TRUE (the default), failure will also occur with any of the following conditions:</p><ul><li>No media was found in the device.</li><li>Media does not contain audio tracks.</li></ul><h4 class=CHeading>Remarks</h4><p>After the device has been successfully opened, the time format is set to milliseconds which will remain in effect until it is manually set to another value or until the device is closed.</p></div></div></div>

<div class="CFunction"><div class=CTopic><h3 class=CTitle><a name="MCI_Length"></a>MCI_Length</h3><div class=CBody><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_Length(</td><td class=PParameter nowrap>p_lpszDeviceID,</td><td class=PDefaultValuePrefix>&nbsp;&nbsp;</td></tr><tr><td></td><td class=PParameter nowrap>p_Track</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote><h4 class=CHeading>Description</h4><p>Gets the total length of the media in the current time format.</p><h4 class=CHeading>Parameters</h4><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>p_lpszDeviceID</td><td class=CDLDescription>Device name or alias.</td></tr><tr><td class=CDLEntry>p_Track</td><td class=CDLDescription>Track number.&nbsp; [Optional] The default is 0 (no track number).</td></tr></table><h4 class=CHeading>Returns</h4><p>If a track number is not specified (the default), the length of the entire media is returned.&nbsp;  If a track number is specified, only the the length of the specified track is returned.</p></div></div></div>

<div class="CFunction"><div class=CTopic><h3 class=CTitle><a name="MCI_MediaIsPresent"></a>MCI_MediaIsPresent</h3><div class=CBody><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_MediaIsPresent(</td><td class=PParameter nowrap>p_lpszDeviceID</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote><h4 class=CHeading>Description</h4><p>Checks to see if media is present in the device.</p><h4 class=CHeading>Parameters</h4><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>p_lpszDeviceID</td><td class=CDLDescription>Device name or alias.</td></tr></table><h4 class=CHeading>Returns</h4><p>TRUE if the media is inserted in the device, otherwise FALSE. msdn: Sequencer, video-overlay, digital-video, and waveform-audio devices (always) return TRUE.</p></div></div></div>

<div class="CFunction"><div class=CTopic><h3 class=CTitle><a name="MCI_Notify"></a>MCI_Notify</h3><div class=CBody><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_Notify(</td><td class=PParameter nowrap>wParam,</td></tr><tr><td></td><td class=PParameter nowrap>lParam,</td></tr><tr><td></td><td class=PParameter nowrap>msg,</td></tr><tr><td></td><td class=PParameter nowrap>hWnd</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote><h4 class=CHeading>Description</h4><p>(Internal function.&nbsp;  Do not call directly)</p><p>This function has 2 responsibilties...</p><p>1) If called by the <a href="#MCI_Play" class=LFunction id=link30 onMouseOver="ShowTip(event, 'tt11', 'link30')" onMouseOut="HideTip('tt11')">MCI_Play</a> function, wParam contains the name of the developer-defined function.&nbsp;  This value is assigned to the s_Callback static variable for future use.</p><p>2) When called as a result of MM_MCINOTIFY message, this function will call the developer-defined function (name stored in the s_Callback static variable) sending the MM_MCINOTIFY status flag as the first parameter.</p><h4 class=CHeading>Parameters</h4><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>wParam</td><td class=CDLDescription>Function name or a MM_MCINOTIFY flag.</td></tr></table><p>MM_MCINOTIFY flag values are as follows...</p><blockquote><pre>MCI_NOTIFY_SUCCESSFUL:=0x1
    The conditions initiating the callback function have been met.

MCI_NOTIFY_SUPERSEDED:=0x2
    The device received another command with the &quot;notify&quot; flag set
    and the current conditions for initiating the callback function
    have been superseded.

MCI_NOTIFY_ABORTED:=0x4
    The device received a command that prevented the current
    conditions for initiating the callback function from being met.
    If a new command interrupts the current command and  it also
    requests notification, the device sends this message only and
    not MCI_NOTIFY_SUPERSEDED.

MCI_NOTIFY_FAILURE:=0x8
    A device error occurred while the device was executing the
    command.</pre></blockquote><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>lParam</td><td class=CDLDescription>lDevID.&nbsp;  This is the identifier of the device initiating the callback function.&nbsp;  This information is only useful if operating more than one MCI device at a time.</td></tr></table><h4 class=CHeading>Returns</h4><p>Per msdn, returns 0 to indicate a successful call.</p><h4 class=CHeading>Remarks</h4><p>This function does not complete until the call to the developer-defined function has completed.&nbsp;  If a MM_MCINOTIFY message is issued while this function is running, the message will be treated as unmonitored.</p></div></div></div>

<div class="CFunction"><div class=CTopic><h3 class=CTitle><a name="MCI_NumberOfTracks"></a>MCI_NumberOfTracks</h3><div class=CBody><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_NumberOfTracks(</td><td class=PParameter nowrap>p_lpszDeviceID</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote><h4 class=CHeading>Description</h4><p>Identifies the number of tracks on the media.</p><h4 class=CHeading>Parameters</h4><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>p_lpszDeviceID</td><td class=CDLDescription>Device name or alias.</td></tr></table><h4 class=CHeading>Returns</h4><p>The number of tracks on the media.</p><h4 class=CHeading>Remarks</h4><p>msdn: The MCISEQ and MCIWAVE devices return 1, as do most VCR devices.&nbsp; The MCIPIONR device does not support this flag.</p></div></div></div>

<div class="CFunction"><div class=CTopic><h3 class=CTitle><a name="MCI_Pause"></a>MCI_Pause</h3><div class=CBody><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_Pause(</td><td class=PParameter nowrap>p_lpszDeviceID</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote><h4 class=CHeading>Description</h4><p>Pauses playback or recording.</p><h4 class=CHeading>Parameters</h4><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>p_lpszDeviceID</td><td class=CDLDescription>Device name or alias.</td></tr></table><h4 class=CHeading>Returns</h4><p>The return code from the <a href="#MCI_SendString" class=LFunction id=link31 onMouseOver="ShowTip(event, 'tt24', 'link31')" onMouseOut="HideTip('tt24')">MCI_SendString</a> function which is 0 if the command completed successfully.</p><h4 class=CHeading>Remarks</h4><p>msdn: With the MCICDA, MCISEQ, and MCIPIONR drivers, the pause command works the same as the stop command.</p><p>Observation: For MCISEQ devices, pause works OK for me.</p></div></div></div>

<div class="CFunction"><div class=CTopic><h3 class=CTitle><a name="MCI_Play"></a>MCI_Play</h3><div class=CBody><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_Play(</td><td class=PParameter nowrap>p_lpszDeviceID,</td><td class=PDefaultValuePrefix>&nbsp;&nbsp;</td><td class=PDefaultValue width=100%></td></tr><tr><td></td><td class=PParameter nowrap>p_Flags</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>&quot;&quot;,</td></tr><tr><td></td><td class=PParameter nowrap>p_Callback</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>&quot;&quot;,</td></tr><tr><td></td><td class=PParameter nowrap>p_hwndCallback</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>0</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote><h4 class=CHeading>Description</h4><p>Starts playing a device.</p><h4 class=CHeading>Parameters</h4><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>p_lpszDeviceID</td><td class=CDLDescription>Device name or alias.</td></tr><tr><td class=CDLEntry>p_Flags</td><td class=CDLDescription>Flags that determine how the device is played.&nbsp; [Optional] If blank, no flags are used.</td></tr></table><h4 class=CHeading>Flag Notes</h4><p>Some commonly used flags include...</p><blockquote><pre>from {position}
to {position}</pre></blockquote><p>If more than one flag is used, separate each flag/value with a space.&nbsp;  For example:</p><blockquote><pre>from 10144 to 95455</pre></blockquote><p>Additional notes...</p><ul><li>With the exception of very short sound files (&lt;300 ms), the &ldquo;wait&rdquo; flag is not recommended.&nbsp;  The entire application will be non-responsive while the media is being played.</li><li>Do not add the &ldquo;notify&rdquo; flag unless you plan to have your script trap the MM_MCINOTIFY message outside of this function.&nbsp; The &ldquo;notify&rdquo; flag is automatically added if the p_Callback parameter contains a value.</li><li>For a complete list of flags and descriptions for the &ldquo;play&rdquo; command string, see the &ldquo;MCI Reference Guide&rdquo; in the <a href="#Links" class=LGroup id=link32 onMouseOver="ShowTip(event, 'tt25', 'link32')" onMouseOut="HideTip('tt25')">Links</a> section.</li></ul><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>p_Callback</td><td class=CDLDescription>Function name that is called when the MM_MCINOTIFY message is sent.&nbsp; [Optional] If defined, the &ldquo;notify&rdquo; flag is automatically added.</td></tr></table><p>Important:  The syntax of this parameter and the associated function is critical.&nbsp;  If not defined correctly, the script may crash.</p><p>The function must have at least one parameter.&nbsp;  For example...</p><blockquote><pre>MyNotifyFunction(NotifyFlag)</pre></blockquote><p>Additional parameters are allowed but they must be optional (contain a default value).&nbsp;  For example:</p><blockquote><pre>MyNotifyFunction(NotifyFlag,FirstCall=False,Parm3=&quot;ABC&quot;)</pre></blockquote><p>When a notify message is sent, the approriate MM_MCINOTIFY flag is sent to the developer-defined function as the first parameter.&nbsp;  See the <a href="#MCI_Notify" class=LFunction id=link33 onMouseOver="ShowTip(event, 'tt8', 'link33')" onMouseOut="HideTip('tt8')">MCI_Notify</a> function for a description and a list of MM_MCINOTIFY flag values.</p><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>p_hWndCallback</td><td class=CDLDescription>Handle to a callback window if the p_Callback parameter contains a value and/or if the &ldquo;notify&rdquo; flag is defined.&nbsp; [Optional]  If undefined but needed, the handle to default Autohotkey window is used.</td></tr></table><h4 class=CHeading>Returns</h4><p>The return code from the <a href="#MCI_SendString" class=LFunction id=link34 onMouseOver="ShowTip(event, 'tt24', 'link34')" onMouseOut="HideTip('tt24')">MCI_SendString</a> function which is 0 if the command completed successfully.</p></div></div></div>

<div class="CFunction"><div class=CTopic><h3 class=CTitle><a name="MCI_Position"></a>MCI_Position</h3><div class=CBody><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_Position(</td><td class=PParameter nowrap>p_lpszDeviceID,</td><td class=PDefaultValuePrefix>&nbsp;&nbsp;</td></tr><tr><td></td><td class=PParameter nowrap>p_Track</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote><h4 class=CHeading>Description</h4><p>Identifies the current playback or recording position.</p><h4 class=CHeading>Parameters</h4><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>p_lpszDeviceID</td><td class=CDLDescription>Device name or alias.</td></tr><tr><td class=CDLEntry>p_Track</td><td class=CDLDescription>Track number.&nbsp; [Optional] The default is 0 (no track number).</td></tr></table><h4 class=CHeading>Returns</h4><p>The current playback or recording position in the current time format.&nbsp; If the p_Track parameter contains a non-zero value, the start position of the track relative to entire media is returned.</p></div></div></div>

<div class="CFunction"><div class=CTopic><h3 class=CTitle><a name="MCI_Record"></a>MCI_Record</h3><div class=CBody><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_Record(</td><td class=PParameter nowrap>p_lpszDeviceID,</td><td class=PDefaultValuePrefix>&nbsp;&nbsp;</td><td class=PDefaultValue width=100%></td></tr><tr><td></td><td class=PParameter nowrap>p_Flags</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>&quot;&quot;</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote><h4 class=CHeading>Description</h4><p>Starts recording.</p><h4 class=CHeading>Parameters</h4><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>p_lpszDeviceID</td><td class=CDLDescription>Device name or alias.</td></tr><tr><td class=CDLEntry>p_Flags</td><td class=CDLDescription>Flags that determine how the device operates for recording.&nbsp; [Optional] If blank, no flags are used.</td></tr></table><h4 class=CHeading>Flag Notes</h4><p>Some commonly used flags include...</p><blockquote><pre>from {position}
to {position}
insert
overwrite</pre></blockquote><p>If more than one flag is used, separate each flag/value with a space.&nbsp;  For example:</p><blockquote><pre>overwrite from 18122 to 26427</pre></blockquote><p>Additional notes...</p><ul><li>The &ldquo;wait&rdquo; flag is not recommended.&nbsp;  The entire application will be non-responsive until recording is stopped with a Stop or Pause command.</li><li>For a complete list of flags and descriptions for the &ldquo;record&rdquo; command string, see the &ldquo;MCI Reference Guide&rdquo; in the <a href="#Links" class=LGroup id=link35 onMouseOver="ShowTip(event, 'tt25', 'link35')" onMouseOut="HideTip('tt25')">Links</a> section.</li></ul><h4 class=CHeading>Returns</h4><p>The return code from the <a href="#MCI_SendString" class=LFunction id=link36 onMouseOver="ShowTip(event, 'tt24', 'link36')" onMouseOut="HideTip('tt24')">MCI_SendString</a> function which is 0 if the command completed successfully.</p><h4 class=CHeading>Remarks</h4><p>msdn: Recording stops when a Stop or Pause command is issued.&nbsp;  For the MCIWAVE driver, all data recorded after a file is opened is discarded if the file is closed without saving it.</p><h4 class=CHeading>Credit</h4><p>Original function and examples by heresy.</p></div></div></div>

<div class="CFunction"><div class=CTopic><h3 class=CTitle><a name="MCI_Resume"></a>MCI_Resume</h3><div class=CBody><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_Resume(</td><td class=PParameter nowrap>p_lpszDeviceID</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote><h4 class=CHeading>Description</h4><p>Resumes playback or recording after the device has been paused.&nbsp;  See the <a href="#MCI_Pause" class=LFunction id=link37 onMouseOver="ShowTip(event, 'tt10', 'link37')" onMouseOut="HideTip('tt10')">MCI_Pause</a> function for more information.</p><h4 class=CHeading>Parameters</h4><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>p_lpszDeviceID</td><td class=CDLDescription>Device name or alias.</td></tr></table><h4 class=CHeading>Returns</h4><p>The return code from the <a href="#MCI_SendString" class=LFunction id=link38 onMouseOver="ShowTip(event, 'tt24', 'link38')" onMouseOut="HideTip('tt24')">MCI_SendString</a> function which is 0 if the command completed successfully.</p><h4 class=CHeading>Remarks</h4><p>msdn: Digital-video, VCR, and waveform-audio devices recognize this command.&nbsp; Although CD audio, MIDI sequencer, and videodisc devices also recognize this command, the MCICDA, MCISEQ, and MCIPIONR device drivers do not support it.</p><h4 class=CHeading>Programming Notes</h4><p>The <a href="#MCI_Play" class=LFunction id=link39 onMouseOver="ShowTip(event, 'tt11', 'link39')" onMouseOut="HideTip('tt11')">MCI_Play</a> function can sometimes be an alternative to this function.&nbsp;  Many devices will begin to play where they were last paused.&nbsp; If the device does not begin playback correctly, try specifying an appropriate &ldquo;From&rdquo; and &ldquo;To&rdquo; value (if needed) in the p_Flags parameter.</p></div></div></div>

<div class="CFunction"><div class=CTopic><h3 class=CTitle><a name="MCI_Save"></a>MCI_Save</h3><div class=CBody><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_Save(</td><td class=PParameter nowrap>p_lpszDeviceID,</td></tr><tr><td></td><td class=PParameter nowrap>p_FileName</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote><h4 class=CHeading>Description</h4><p>Saves an MCI file.</p><h4 class=CHeading>Parameters</h4><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>p_lpszDeviceID</td><td class=CDLDescription>Device name or alias.</td></tr><tr><td class=CDLEntry>p_FileName</td><td class=CDLDescription>File name to store a MCI file.&nbsp;  If the file does not exist, a new file will be created.&nbsp;  If the file exists, it will be overwritten.</td></tr></table><h4 class=CHeading>Returns</h4><p>The return code from the <a href="#MCI_SendString" class=LFunction id=link40 onMouseOver="ShowTip(event, 'tt24', 'link40')" onMouseOut="HideTip('tt24')">MCI_SendString</a> function which is 0 if the command completed successfully.</p><h4 class=CHeading>Remarks</h4><p>This command can overwrite existing files.&nbsp;  Use with care.</p><h4 class=CHeading>Credit</h4><p>Original function and examples by heresy.</p></div></div></div>

<div class="CFunction"><div class=CTopic><h3 class=CTitle><a name="MCI_Seek"></a>MCI_Seek</h3><div class=CBody><h4 class=CHeading>Description</h4><p>Move to a specified position.</p><h4 class=CHeading>Parameters</h4><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>p_lpszDeviceID</td><td class=CDLDescription>Device name or alias.</td></tr><tr><td class=CDLEntry>p_Position</td><td class=CDLDescription>Position to stop the seek.&nbsp;  Value must be &ldquo;start&rdquo;, &ldquo;end&rdquo;, or an integer.</td></tr></table><h4 class=CHeading>Returns</h4><p>The return code from the <a href="#MCI_SendString" class=LFunction id=link41 onMouseOver="ShowTip(event, 'tt24', 'link41')" onMouseOut="HideTip('tt24')">MCI_SendString</a> function which is 0 if the command completed successfully.</p></div></div></div>

<div class="CFunction"><div class=CTopic><h3 class=CTitle><a name="MCI_SetBass"></a>MCI_SetBass</h3><div class=CBody><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_SetBass(</td><td class=PParameter nowrap>p_lpszDeviceID,</td></tr><tr><td></td><td class=PParameter nowrap>p_Factor</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote><h4 class=CHeading>Description</h4><p>Sets the audio low frequency level.</p><h4 class=CHeading>Parameters</h4><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>p_lpszDeviceID</td><td class=CDLDescription>Device name or alias.</td></tr><tr><td class=CDLEntry>p_Factor</td><td class=CDLDescription>Bass factor.</td></tr></table><h4 class=CHeading>Returns</h4><p>The return code from the <a href="#MCI_SendString" class=LFunction id=link42 onMouseOver="ShowTip(event, 'tt24', 'link42')" onMouseOut="HideTip('tt24')">MCI_SendString</a> function which is 0 if the command completed successfully.</p><h4 class=CHeading>Observations</h4><ul><li>Factor range appears to be from 0 to ?????.</li><li>Most MCI devices do not support this command.</li></ul></div></div></div>

<div class="CFunction"><div class=CTopic><h3 class=CTitle><a name="MCI_SetTreble"></a>MCI_SetTreble</h3><div class=CBody><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_SetTreble(</td><td class=PParameter nowrap>p_lpszDeviceID,</td></tr><tr><td></td><td class=PParameter nowrap>p_Factor</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote><h4 class=CHeading>Description</h4><p>Sets the audio high-frequency level.</p><h4 class=CHeading>Parameters</h4><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>p_lpszDeviceID</td><td class=CDLDescription>Device name or alias.</td></tr><tr><td class=CDLEntry>p_Factor</td><td class=CDLDescription>Treble factor.</td></tr></table><h4 class=CHeading>Returns</h4><p>The return code from the <a href="#MCI_SendString" class=LFunction id=link43 onMouseOver="ShowTip(event, 'tt24', 'link43')" onMouseOut="HideTip('tt24')">MCI_SendString</a> function which is 0 if the command completed successfully.</p><h4 class=CHeading>Observations</h4><ul><li>Factor range appears to be from 0 to ?????.</li><li>Most MCI devices do not support this command.</li></ul></div></div></div>

<div class="CFunction"><div class=CTopic><h3 class=CTitle><a name="MCI_SetVolume"></a>MCI_SetVolume</h3><div class=CBody><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_SetVolume(</td><td class=PParameter nowrap>p_lpszDeviceID,</td></tr><tr><td></td><td class=PParameter nowrap>p_Factor</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote><h4 class=CHeading>Description</h4><p>Sets the average audio volume for both audio channels.&nbsp; If the left and right volumes have been set to different values, then the ratio of left-to-right volume is approximately unchanged.</p><h4 class=CHeading>Parameters</h4><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>p_lpszDeviceID</td><td class=CDLDescription>Device name or alias.</td></tr><tr><td class=CDLEntry>p_Factor</td><td class=CDLDescription>Volume factor.</td></tr></table><h4 class=CHeading>Returns</h4><p>The return code from the <a href="#MCI_SendString" class=LFunction id=link44 onMouseOver="ShowTip(event, 'tt24', 'link44')" onMouseOut="HideTip('tt24')">MCI_SendString</a> function which is 0 if the command completed successfully.</p><h4 class=CHeading>Observations</h4><ul><li>Factor range appears to be from 0 to 1000.</li><li>Most MCI devices do not support this command.</li></ul></div></div></div>

<div class="CFunction"><div class=CTopic><h3 class=CTitle><a name="MCI_Status"></a>MCI_Status</h3><div class=CBody><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_Status(</td><td class=PParameter nowrap>p_lpszDeviceID</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote><h4 class=CHeading>Description</h4><p>Identifies the current mode of the device.</p><h4 class=CHeading>Parameters</h4><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>p_lpszDeviceID</td><td class=CDLDescription>Device name or alias.</td></tr></table><h4 class=CHeading>Returns</h4><p>The current mode of the device.</p><p>msdn: All devices can return the &ldquo;not ready&rdquo;, &ldquo;paused&rdquo;, &ldquo;playing&rdquo;, and &ldquo;stopped&rdquo; values.&nbsp; Some devices can return the additional &ldquo;open&rdquo;, &ldquo;parked&rdquo;, &ldquo;recording&rdquo;, and &ldquo;seeking&rdquo; values.</p></div></div></div>

<div class="CFunction"><div class=CTopic><h3 class=CTitle><a name="MCI_Stop"></a>MCI_Stop</h3><div class=CBody><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_Stop(</td><td class=PParameter nowrap>p_lpszDeviceID</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote><h4 class=CHeading>Description</h4><p>Stops playback or recording.</p><h4 class=CHeading>Parameters</h4><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>p_lpszDeviceID</td><td class=CDLDescription>Device name or alias.</td></tr></table><h4 class=CHeading>Returns</h4><p>The return code from the <a href="#MCI_SendString" class=LFunction id=link45 onMouseOver="ShowTip(event, 'tt24', 'link45')" onMouseOut="HideTip('tt24')">MCI_SendString</a> function which is 0 if the command completed successfully.</p><h4 class=CHeading>Remarks</h4><ul><li>After close, a &ldquo;seek to start&rdquo; is not done because  1) it slows down the stop request and  2) it may be unwanted.&nbsp;  If you need to set the media position back to the beginning after a stop, call the <a href="#MCI_Seek" class=LFunction id=link46 onMouseOver="ShowTip(event, 'tt26', 'link46')" onMouseOut="HideTip('tt26')">MCI_Seek</a> function and set the p_Position parameter to 0.</li><li>For (some) CD audio devices, the stop command stops playback and resets the current track position to zero.</li></ul></div></div></div>

<div class="CFunction"><div class=CTopic><h3 class=CTitle><a name="MCI_TrackIsAudio"></a>MCI_TrackIsAudio</h3><div class=CBody><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_TrackIsAudio(</td><td class=PParameter nowrap>p_lpszDeviceID,</td><td class=PDefaultValuePrefix>&nbsp;&nbsp;</td><td class=PDefaultValue width=100%></td></tr><tr><td></td><td class=PParameter nowrap>p_Track</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>1</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote><h4 class=CHeading>Description</h4><p>Determines if the specified track is an audio track.</p><h4 class=CHeading>Parameters</h4><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>p_lpszDeviceID</td><td class=CDLDescription>Device name or alias.</td></tr><tr><td class=CDLEntry>p_Track</td><td class=CDLDescription>Track number.&nbsp; [Optional] The default is 1.</td></tr></table><h4 class=CHeading>Returns</h4><p>TRUE if the specified track is an audio track, otherwise FALSE.</p><h4 class=CHeading>Remarks</h4><p>This command will only work on a device that supports multiple tracks.</p></div></div></div>

<div class="CFunction"><div class=CTopic><h3 class=CTitle><a name="MCI_ToHHMMSS"></a>MCI_ToHHMMSS</h3><div class=CBody><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_ToHHMMSS(</td><td class=PParameter nowrap>p_ms,</td><td class=PDefaultValuePrefix>&nbsp;&nbsp;</td><td class=PDefaultValue width=100%></td></tr><tr><td></td><td class=PParameter nowrap>p_MinimumSize</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>4</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote><h4 class=CHeading>Description</h4><p>Converts the specified number of milliseconds to hh:mm:ss format.</p><h4 class=CHeading>Parameters</h4><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>p_ms</td><td class=CDLDescription>Number of milliseconds.</td></tr><tr><td class=CDLEntry>p_MinimumSize</td><td class=CDLDescription>Minimum size.&nbsp;  [Optional] The default is 4.&nbsp;  This is the minimum size in characters (not significant digits) that is returned.&nbsp;  Unless you want a &ldquo;:&rdquo; character to show as the leading character, don&rsquo;t set this value to 3 or 6.</td></tr></table><h4 class=CHeading>Returns</h4><p>The amount of time in hh:mm:ss format with leading zero and &ldquo;:&rdquo; characters suppressed unless the length is less than p_MinimumSize.&nbsp; Note:  If the number of hours is greater than 99, the size of hour (&ldquo;hh&rdquo;) will increase as needed.</p><h4 class=CHeading>Usage Notes</h4><p>To use this function to create separate variables for the number of hours, minutes, and seconds, set the p_MinimumSize parameter to 8 and use simple <b>SubStr</b> commands to create these variables.&nbsp;  For example:</p><blockquote><pre>x:=MCI_ToHHMMSS(NumberOfMilliseconds,8)
HH:=SubStr(x,1,2)
MM:=SubStr(x,4,2)
SS:=SubStr(x,6,2)</pre></blockquote><p>To remove leading zeros from these variables, simply add 0 to the extracted value.&nbsp;  For example:</p><blockquote><pre>MM:=SubStr(x,4,2)+0</pre></blockquote><h4 class=CHeading>Credit</h4><p>This function is a customized version of an example that was extracted from the AutoHotkey documenation.</p></div></div></div>

<div class="CFunction"><div class=CTopic><h3 class=CTitle><a name="MCI_ToMilliseconds"></a>MCI_ToMilliseconds</h3><div class=CBody><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_ToMilliseconds(</td><td class=PParameter nowrap>Hour,</td></tr><tr><td></td><td class=PParameter nowrap>Min,</td></tr><tr><td></td><td class=PParameter nowrap>Sec</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote><h4 class=CHeading>Description</h4><p>Converts the specified hour, minute and second into a valid milliseconds timestamp.</p><h4 class=CHeading>Parameters</h4><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>Hour, Min, Sec</td><td class=CDLDescription>Position to convert to milliseconds</td></tr></table><h4 class=CHeading>Returns</h4><p>The specified position converted to milliseconds.</p></div></div></div>

<div class="CFunction"><div class=CTopic><h3 class=CTitle><a name="MCI_SendString"></a>MCI_SendString</h3><div class=CBody><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_SendString(</td><td class=PType nowrap>&nbsp;</td><td class=PParameter nowrap>p_lpszCommand,</td><td class=PDefaultValuePrefix>&nbsp;&nbsp;</td><td class=PDefaultValue width=100%></td></tr><tr><td></td><td class=PType nowrap>ByRef&nbsp;</td><td class=PParameter nowrap>r_lpszReturnString</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>&quot;&quot;,</td></tr><tr><td></td><td class=PType nowrap>&nbsp;</td><td class=PParameter nowrap>p_hwndCallback</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>0</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote><h4 class=CHeading>Description</h4><p>This is the primary function that controls MCI operations.&nbsp;  With the exception of formatting functions, all of the functions in this library call this function.</p><h4 class=CHeading>Parameters</h4><table border=0 cellspacing=0 cellpadding=0 class=CDescriptionList><tr><td class=CDLEntry>p_lpszCommand</td><td class=CDLDescription>MCI command string.</td></tr><tr><td class=CDLEntry>r_lpszReturnString</td><td class=CDLDescription>Variable name that receives return information.&nbsp; [Optional]</td></tr><tr><td class=CDLEntry>p_hwndCallback</td><td class=CDLDescription>Handle to a callback window if the &ldquo;notify&rdquo; flag was specified in the command string.&nbsp;  [Optional] The default is 0 (No callback window).</td></tr></table><h4 class=CHeading>Returns</h4><p>Two values are returned.</p><p>1) The function returns 0 if successful or an error number otherwise.</p><p>2) If the MCI command string was a request for information, the variable named in the r_lpszReturnString parameter will contain the requested information.</p><h4 class=CHeading>Debugging</h4><p>If a non-zero value is returned from the call to the mciSendString API function, a call to the mciGetErrorString API function is made to convert the error number into a developer-friendly error message.&nbsp;  All of this information is sent to the debugger in an easy-to-read format.</p></div></div></div>

</div><!--Content-->


<div id=Footer><a href="http://www.naturaldocs.org">Generated by Natural Docs</a></div><!--Footer-->






<!--START_ND_TOOLTIPS-->
<div class=CToolTip id="tt1"><div class=CFunction><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_Close(</td><td class=PParameter nowrap>p_lpszDeviceID</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote>Closes the device and any associated resources.</div></div><div class=CToolTip id="tt2"><div class=CFunction><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_CurrentTrack(</td><td class=PParameter nowrap>p_lpszDeviceID</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote>Identifies the current track.</div></div><div class=CToolTip id="tt3"><div class=CFunction><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_DeviceType(</td><td class=PParameter nowrap>p_lpszDeviceID</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote>Identifies the device type name.</div></div><div class=CToolTip id="tt4"><div class=CFunction><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_Open(</td><td class=PParameter nowrap>p_MediaFile,</td><td class=PDefaultValuePrefix>&nbsp;&nbsp;</td><td class=PDefaultValue width=100%></td></tr><tr><td></td><td class=PParameter nowrap>p_Alias</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>&quot;&quot;,</td></tr><tr><td></td><td class=PParameter nowrap>p_Flags</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>&quot;&quot;</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote>Opens an MCI device and loads the specified file.</div></div><div class=CToolTip id="tt5"><div class=CFunction><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_OpenCDAudio(</td><td class=PParameter nowrap>p_Drive</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>&quot;&quot;,</td></tr><tr><td></td><td class=PParameter nowrap>p_Alias</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>&quot;&quot;,</td></tr><tr><td></td><td class=PParameter nowrap>p_CheckForMedia</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>True</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote>Opens a CDAudio device.</div></div><div class=CToolTip id="tt6"><div class=CFunction><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_Length(</td><td class=PParameter nowrap>p_lpszDeviceID,</td><td class=PDefaultValuePrefix>&nbsp;&nbsp;</td></tr><tr><td></td><td class=PParameter nowrap>p_Track</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote>Gets the total length of the media in the current time format.</div></div><div class=CToolTip id="tt7"><div class=CFunction><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_MediaIsPresent(</td><td class=PParameter nowrap>p_lpszDeviceID</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote>Checks to see if media is present in the device.</div></div><div class=CToolTip id="tt8"><div class=CFunction><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_Notify(</td><td class=PParameter nowrap>wParam,</td></tr><tr><td></td><td class=PParameter nowrap>lParam,</td></tr><tr><td></td><td class=PParameter nowrap>msg,</td></tr><tr><td></td><td class=PParameter nowrap>hWnd</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote>(Internal function. </div></div><div class=CToolTip id="tt9"><div class=CFunction><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_NumberOfTracks(</td><td class=PParameter nowrap>p_lpszDeviceID</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote>Identifies the number of tracks on the media.</div></div><div class=CToolTip id="tt10"><div class=CFunction><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_Pause(</td><td class=PParameter nowrap>p_lpszDeviceID</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote>Pauses playback or recording.</div></div><div class=CToolTip id="tt11"><div class=CFunction><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_Play(</td><td class=PParameter nowrap>p_lpszDeviceID,</td><td class=PDefaultValuePrefix>&nbsp;&nbsp;</td><td class=PDefaultValue width=100%></td></tr><tr><td></td><td class=PParameter nowrap>p_Flags</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>&quot;&quot;,</td></tr><tr><td></td><td class=PParameter nowrap>p_Callback</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>&quot;&quot;,</td></tr><tr><td></td><td class=PParameter nowrap>p_hwndCallback</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>0</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote>Starts playing a device.</div></div><div class=CToolTip id="tt12"><div class=CFunction><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_Position(</td><td class=PParameter nowrap>p_lpszDeviceID,</td><td class=PDefaultValuePrefix>&nbsp;&nbsp;</td></tr><tr><td></td><td class=PParameter nowrap>p_Track</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote>Identifies the current playback or recording position.</div></div><div class=CToolTip id="tt13"><div class=CFunction><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_Record(</td><td class=PParameter nowrap>p_lpszDeviceID,</td><td class=PDefaultValuePrefix>&nbsp;&nbsp;</td><td class=PDefaultValue width=100%></td></tr><tr><td></td><td class=PParameter nowrap>p_Flags</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>&quot;&quot;</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote>Starts recording.</div></div><div class=CToolTip id="tt14"><div class=CFunction><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_Resume(</td><td class=PParameter nowrap>p_lpszDeviceID</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote>Resumes playback or recording after the device has been paused. </div></div><div class=CToolTip id="tt15"><div class=CFunction><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_Save(</td><td class=PParameter nowrap>p_lpszDeviceID,</td></tr><tr><td></td><td class=PParameter nowrap>p_FileName</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote>Saves an MCI file.</div></div><div class=CToolTip id="tt16"><div class=CFunction><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_SetBass(</td><td class=PParameter nowrap>p_lpszDeviceID,</td></tr><tr><td></td><td class=PParameter nowrap>p_Factor</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote>Sets the audio low frequency level.</div></div><div class=CToolTip id="tt17"><div class=CFunction><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_SetTreble(</td><td class=PParameter nowrap>p_lpszDeviceID,</td></tr><tr><td></td><td class=PParameter nowrap>p_Factor</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote>Sets the audio high-frequency level.</div></div><div class=CToolTip id="tt18"><div class=CFunction><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_SetVolume(</td><td class=PParameter nowrap>p_lpszDeviceID,</td></tr><tr><td></td><td class=PParameter nowrap>p_Factor</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote>Sets the average audio volume for both audio channels. </div></div><div class=CToolTip id="tt19"><div class=CFunction><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_Status(</td><td class=PParameter nowrap>p_lpszDeviceID</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote>Identifies the current mode of the device.</div></div><div class=CToolTip id="tt20"><div class=CFunction><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_Stop(</td><td class=PParameter nowrap>p_lpszDeviceID</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote>Stops playback or recording.</div></div><div class=CToolTip id="tt21"><div class=CFunction><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_TrackIsAudio(</td><td class=PParameter nowrap>p_lpszDeviceID,</td><td class=PDefaultValuePrefix>&nbsp;&nbsp;</td><td class=PDefaultValue width=100%></td></tr><tr><td></td><td class=PParameter nowrap>p_Track</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>1</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote>Determines if the specified track is an audio track.</div></div><div class=CToolTip id="tt22"><div class=CFunction><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_ToHHMMSS(</td><td class=PParameter nowrap>p_ms,</td><td class=PDefaultValuePrefix>&nbsp;&nbsp;</td><td class=PDefaultValue width=100%></td></tr><tr><td></td><td class=PParameter nowrap>p_MinimumSize</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>4</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote>Converts the specified number of milliseconds to hh:mm:ss format.</div></div><div class=CToolTip id="tt23"><div class=CFunction><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_ToMilliseconds(</td><td class=PParameter nowrap>Hour,</td></tr><tr><td></td><td class=PParameter nowrap>Min,</td></tr><tr><td></td><td class=PParameter nowrap>Sec</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote>Converts the specified hour, minute and second into a valid milliseconds timestamp.</div></div><div class=CToolTip id="tt24"><div class=CFunction><blockquote><table border=0 cellspacing=0 cellpadding=0 class=Prototype><tr><td><table border=0 cellspacing=0 cellpadding=0><tr><td class=PBeforeParameters nowrap>MCI_SendString(</td><td class=PType nowrap>&nbsp;</td><td class=PParameter nowrap>p_lpszCommand,</td><td class=PDefaultValuePrefix>&nbsp;&nbsp;</td><td class=PDefaultValue width=100%></td></tr><tr><td></td><td class=PType nowrap>ByRef&nbsp;</td><td class=PParameter nowrap>r_lpszReturnString</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>&quot;&quot;,</td></tr><tr><td></td><td class=PType nowrap>&nbsp;</td><td class=PParameter nowrap>p_hwndCallback</td><td class=PDefaultValuePrefix>&nbsp;=&nbsp;</td><td class=PDefaultValue width=100%>0</td><td class=PAfterParameters nowrap>)</td></tr></table></td></tr></table></blockquote>This is the primary function that controls MCI operations. </div></div><div class=CToolTip id="tt25"><div class=CGroup>MCI Reference Guide</div></div><div class=CToolTip id="tt26"><div class=CFunction>Move to a specified position.</div></div><!--END_ND_TOOLTIPS-->




<div id=MSearchResultsWindow><iframe src="" frameborder=0 name=MSearchResults id=MSearchResults></iframe><a href="javascript:searchPanel.CloseResultsWindow()" id=MSearchResultsWindowClose>Close</a></div>


<script language=JavaScript><!--
if (browserType) {if (browserVer) {document.write("</div>"); }document.write("</div>");}// --></script></body></html>