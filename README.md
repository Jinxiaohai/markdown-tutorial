[TOC]
# Usage  
Keybindings are grouped by prefixes based on their function. For example, the commands for inserting links are grouped
under C-c C-a, where the C-a is a mnemonic for the HTML  tag. In other cases, the connection to HTML is not direct.
For example, commands dealing with headings begin with C-c C-t (mnemonic: titling). The primary commands in each group
will are described below. You can obtain a list of all keybindings by pressing C-c C-h. Movement and shifting commands
tend to be associated with paired delimiters such as M-{ and M-} or C-c \< and C-c \>. Outline navigation keybindings the
same as in org-mode. Finally, commands for running Markdown or doing maintenance on an open file are grouped under the
C-c C-c prefix. The most commonly used commands are described below. You can obtain a list of all keybindings by
pressing C-c C-h.

* Hyperlinks: C-c C-a  
  > C-c C-a l inserts an inline link of the form\[text\](url).  
  > C-c C-a L inserts a reference link of the form \[text\](label) and, optionally, a corresponding reference label
    definition.  
  > C-c C-a u inserts a bare url, delimited by angle brackets.  
  > C-c C-a f inserts a footnote marker at the point.  
  > C-c C-a w behaves much like the inline link insertion command and inserts a wiki link of the form [[WikiLink]].  
* Images: C-c C-i  
  > C-c C-i i inserts markup for an inline image, using the active region or the word at point, if any, as the alt text.  
  Markdown  
	  
