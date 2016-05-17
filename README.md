# Template for xxxi Mails

## General Structure
```html
<table>
	<tr>
		<td>
			<div>
				<table>
				<!-- start of sections -->
				
				<tr>
					<td>
						<center>
							<table class=“[…] section-number”>
								<tr>
									<td>
										<div class=“cells”>

											<div class=“left x-two/x-one/x-three”
												CONTENT
											</div>
											
											<div class="between">
								                        <table>
								                          <tr>
								                            <td>
								                            </td>
								                          <tr>
								                        </table>
								                      </div>

											<div class=“right x-two/x-one/x-three”>
												CONTENT
											</div>

										</div>
									</td>
									<td class=“expander”></td>
								</tr>
							</table>
						</center>
					</td>
				</tr>

				[…]

				<!-- end of sections -->
				</table>
			</div>
		</td>
	</tr>
</table>
```


## Main classes for structure

### section-[number]
Defines section structure and is a class of the surrounding content table. Every section is in a own table row of the main table.

### .left | .middle | .right
Class for the inner divs defining the position of the table cell. Every table cell div should have one of the position class

### .between
This div is the middle border between table cells. It contains a table.

### .x-one | .x-two | .x-three
The classes define the segmentation of table cells and the width of them. If the table has only one cell none of this classes is needed. If the table has more than one cells every div that defines a cell needs one of this classes.
* x-one: 1/3 of table size in a two-cell table
* x-two: 2/3 of table size in a two-cell table
* x-three: 1/3 of table size in a three-cell table


## Classes for styling

### .halfwhite
This class is used in the between-div for having not a full middle border. The height can be styled in the CSS with top and height.

### .spacerlg | .spacermd | .spacersm
Inserted as an own table row in a section table this class is a full sized spacer

### .border
Insert this classes to tables and table parts to add borders
* .border-t: border top
* .border-b: border bottom
* .border-l: border left
* .border-r: border right

## Sections
Section examples are implemented in the xxxi-file.
