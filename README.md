# FlexLite

纯CSS轻量级Flexbox布局框架，支持十二栅格布局，多浏览器兼容，Class样式分为两类：

1. ````fview_```` 前缀： 父容器相关样式
2. ````fitem_```` 前缀： 子元素相关样式

# fview 容器样式

## 1.布局方式

### 1.1 水平布局

	fview_horz			# 等同于flex-flow: row nowarp;
	fview_horz_warp		# 等同于flex-flow: row warp;
	fview_horz_-warp	# 等同于flex-flow: row wrap-reverse;
	fview_-horz			# 等同于flex-flow: row-reverse nowarp;
	fview_-horz_warp	# 等同于flex-flow: row-reverse warp;
	fview_-horz_-warp	# 等同于flex-flow: row-reverse wrap-reverse;

### 1.2 垂直布局

	fview_vert			# 等同于flex-flow: column nowarp;
	fview_vert_warp		# 等同于flex-flow: column warp;
	fview_vert_-warp	# 等同于flex-flow: column wrap-reverse;
	fview_-vert			# 等同于flex-flow: column-reverse nowarp;
	fview_-vert_warp	# 等同于flex-flow: column-reverse warp;
	fview_-vert_-warp	# 等同于flex-flow: column-reverse wrap-reverse;

## 2.对齐方式

### 2.1 主轴对齐

	fview_align_end		# 等同于justify-content: flex-end;
	fview_align_start	# 等同于justify-content: flex-start;
	fview_align_center	# 等同于justify-content: center;
	fview_align_around	# 等同于justify-content: space-around;
	fview_align_between	# 等同于justify-content: space-between;
	

### 2.2 交叉轴对齐

	fview_align_cross_end		# 等同于align-items: flex-end;
	fview_align_cross_start		# 等同于align-items: flex-start;
	fview_align_cross_center	# 等同于align-items: center;
	fview_align_cross_stretch	# 等同于align-items: stretch;
	fview_align_cross_baseline	# 等同于align-items: baseline;

### 2.3 换行空间对齐

	fview_align_break_end		# 等同于align-content: flex-end;
	fview_align_break_start		# 等同于align-content: flex-start;
	fview_align_break_center	# 等同于align-content: center;
	fview_align_break_around	# 等同于align-content: space-around;
	fview_align_break_between	# 等同于align-content: space-between;
	fview_align_break_stretch	# 等同于align-content: stretch;

# fitem 元素样式

## 1.对齐方式

	fitem_align_end			# 等同于align-self: flex-end;
	fitem_align_start		# 等同于align-self: flex-start;
	fitem_align_center		# 等同于align-self: center;
	fitem_align_stretch		# 等同于align-self: stretch;
	fitem_align_baseline	# 等同于align-self: baseline;
	
## 2.十二栅格

	# 十二栅格对应宽度比例
	fitem_span_[1 - 12]
	
	# 0： 禁用样式（none）
	fitem_grow_[0 - 12]
	
	# 0： 禁用样式（none）
	fitem_basis_[0 - 12]
	
	# 0： 禁用样式（none）
	fitem_shrink_[0 - 12]

## 3.元素排序

	# 0： 禁用排序（none）
	fitem_sort_[0 - 12]
	
## 4.其它样式

	fitem_basis_min		# 等同于flex-basis: min-content;
	fitem_basis_max		# 等同于flex-basis: max-content;
	fitem_basis_fit		# 等同于flex-basis: fit-content;
	fitem_basis_base	# 等同于flex-basis: content;
	fitem_basis_fill	# 等同于flex-basis: fill;
	fitem_basis_auto	# 等同于flex-basis: auto;
