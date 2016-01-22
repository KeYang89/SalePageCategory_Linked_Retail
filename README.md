# SalePageCategory_Linked_Retail
1. To set up the sales page: go to magmi Value Replacer, enters "Category", an input box will show up, enter the following to generate the sales page:
{{{item.price}>{item.special_price}?{item.Category} .';;Sale':{item.Category}}}
2. After step 1., install this extension to add category on the sales page.
3. If you'd like to add the sales category with more customization on the sidebar, go to the Sale category, in Custom Design > Custom Layout Update, put in:
<reference name="left">
      <block type="cms/block" name="salecategory" before="-">
             <action method="setBlockId"><block_id>salecategory</block_id></action>
     </block>
 </reference>
4. In CMS > Static Block, create a static block named salecategory, and put the category hierachy there, each category url should end with "?sale=1"
