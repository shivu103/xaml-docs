---
title: Applied IValueConverter on the DataMemberBinding
page_title: Applied IValueConverter on the DataMemberBinding
description: Applied IValueConverter on the DataMemberBinding
slug: gridview-filtering-faq-ivalueconverter-and-filtering
tags: applied,ivalueconverter,on,the,datamemberbinding
published: True
position: 1
---

# Applied IValueConverter on the DataMemberBinding



## Why isn’t this converter used when performing filtering?
        

__IValueConverters__ are only used for __presentation purposes__. They play absolutely no part in the data engine and __filtering, sorting and grouping are always performed on raw data values__.

Each GridViewColumn has a property called __FilterMemberPath__. You can use this property to tell the column to __filter on a property different from the one it displays__ in its cells. In case the Type of the bound property cannot be automatically discovered by the data engine, you can “help” the column by setting the __FilterMemberType__ property.

>tipFor example: FilterMemberPath="PropertyToFilterOn". You can also check the [FilterMemberPath documentation]({%slug gridview-filtering-basic%}).

# See Also

 * [Basic Filtering]({%slug gridview-filtering-basic%})
