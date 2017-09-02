#### annotate ####
In an annotation, there are two points to consider: the location being annotated
represented by the argument xy and the location of the text xytext. Both of these
arguments are (x, y) tuples.(创建一个文本注释,从指定点指向目标点.)

```python
class matplotlib.text.Annotation(s, xy, xytext=None, xycoords='data', textcoodrs=None,
arrowprops=None, annotation_clip=None, **kwargs)
```
Annotate the point xy with text s.
Additional kwargs are passed to Text.
其中
> s : str
    * the
