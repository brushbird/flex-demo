# flex-demo
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>Flex 布局示例</title>
    <link rel="stylesheet" type="text/css" href="style.css">
</head>

<body>
    <h1>Flex 布局示例</h1>
    <p>感谢阮一峰老师的教程<a target="_blank" href="http://www.ruanyifeng.com/blog/2015/07/flex-grammar.html">http://www.ruanyifeng.com/blog/2015/07/flex-grammar.html</a>
        <br>本示例在网友<a target="_blank" href="http://vgee.cn/">JailBreak</a>所做的<a target="_blank" href="http://static.vgee.cn/static/index.html">Demo</a>的基础上将教程上所有的布局都简单的实现了一遍
        <br>并保存在github上面<a target="_blank" href="https://github.com/brushbird/flex-demo">https://github.com/brushbird/flex-demo</a>
    </p>
    <h2>容器的属性</h2>
    <h3>1、flex-direction属性</h3>
    <p>flex-direction属性决定主轴的方向（即项目的排列方向）。</p>
    <p>
        .box { flex-direction: row | row-reverse | column | column-reverse; }
    </p>
    <div class="tab" js-tab="1">
        <div class="tab-title">
            <a href="javascript:;" class="item item-cur">row</a>
            <a href="javascript:;" class="item">row-reverse</a>
            <a href="javascript:;" class="item">column</a>
            <a href="javascript:;" class="item">column-reverse</a>
        </div>
        <div class="tab-cont">
            <div class="tab-cont__wrap">
                <div class="item">
                    <div class="box box-1-row">
                        <div class="box-item">1</div>
                        <div class="box-item">2</div>
                        <div class="box-item">3</div>
                        <div class="box-item">4</div>
                    </div>
                </div>
                <div class="item">
                    <div class="box box-1-row-reverse">
                        <div class="box-item">1</div>
                        <div class="box-item">2</div>
                        <div class="box-item">3</div>
                        <div class="box-item">4</div>
                    </div>
                </div>
                <div class="item">
                    <div class="box box-1-column">
                        <div class="box-item">1</div>
                        <div class="box-item">2</div>
                        <div class="box-item">3</div>
                        <div class="box-item">4</div>
                    </div>
                </div>
                <div class="item">
                    <div class="box box-1-column-reverse">
                        <div class="box-item">1</div>
                        <div class="box-item">2</div>
                        <div class="box-item">3</div>
                        <div class="box-item">4</div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <h3>2、flex-wrap属性</h3>
    <p>默认情况下，项目都排在一条线（又称"轴线"）上。flex-wrap属性定义，如果一条轴线排不下，如何换行。</p>
    <p>
        .box{ flex-wrap: nowrap | wrap | wrap-reverse; }
    </p>
    <div class="tab" js-tab="2">
        <div class="tab-title">
            <a href="javascript:;" class="item item-cur">nowrap</a>
            <a href="javascript:;" class="item">wrap</a>
            <a href="javascript:;" class="item">wrap-reverse</a>
        </div>
        <div class="tab-cont">
            <div class="tab-cont__wrap">
                <div class="item">
                    <p>nowrap（默认）：不换行。</p>
                    <div class="box box-2">
                        <div class="box-item">1</div>
                        <div class="box-item">2</div>
                        <div class="box-item">3</div>
                        <div class="box-item">4</div>
                        <div class="box-item">5</div>
                        <div class="box-item">6</div>
                        <div class="box-item">7</div>
                    </div>
                </div>
                <div class="item">
                    <p>wrap：换行，第一行在上方。</p>
                    <div class="box box-3">
                        <div class="box-item">1</div>
                        <div class="box-item">2</div>
                        <div class="box-item">3</div>
                        <div class="box-item">4</div>
                        <div class="box-item">5</div>
                        <div class="box-item">6</div>
                        <div class="box-item">7</div>
                    </div>
                </div>
                <div class="item">
                    <p>wrap-reverse：换行，第一行在下方。</p>
                    <div class="box box-4">
                        <div class="box-item">1</div>
                        <div class="box-item">2</div>
                        <div class="box-item">3</div>
                        <div class="box-item">4</div>
                        <div class="box-item">5</div>
                        <div class="box-item">6</div>
                        <div class="box-item">7</div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <h3>3、flex-flow</h3>
    <p>flex-flow属性是flex-direction属性和flex-wrap属性的简写形式，默认值为row nowrap。</p>
    <p>
        .box { flex-flow: &lt;flex-direction&gt; || &lt;flex-wrap&gt;; }
    </p>
    <div class="box box-5">
        <div class="box-item">1</div>
        <div class="box-item">2</div>
        <div class="box-item">3</div>
        <div class="box-item">4</div>
        <div class="box-item">5</div>
        <div class="box-item">6</div>
        <div class="box-item">7</div>
    </div>
    <h3>4、justify-content属性</h3>
    <p>justify-content属性定义了项目在主轴上的对齐方式。</p>
    <p>
        .box { justify-content: flex-start | flex-end | center | space-between | space-around; }
    </p>
    <div class="tab" js-tab="3">
        <div class="tab-title">
            <a href="javascript:;" class="item item-cur">flex-start</a>
            <a href="javascript:;" class="item">flex-end</a>
            <a href="javascript:;" class="item">center</a>
            <a href="javascript:;" class="item">space-between</a>
            <a href="javascript:;" class="item">space-around</a>
        </div>
        <div class="tab-cont">
            <div class="tab-cont__wrap">
                <div class="item">
                    <p>flex-start（默认值）：左对齐</p>
                    <div class="box box-6">
                        <div class="box-item">1</div>
                        <div class="box-item">2</div>
                        <div class="box-item">3</div>
                        <div class="box-item">4</div>
                    </div>
                </div>
                <div class="item">
                    <p>flex-end：右对齐</p>
                    <div class="box box-7">
                        <div class="box-item">1</div>
                        <div class="box-item">2</div>
                        <div class="box-item">3</div>
                        <div class="box-item">4</div>
                    </div>
                </div>
                <div class="item">
                    <p>center： 居中</p>
                    <div class="box box-8">
                        <div class="box-item">1</div>
                        <div class="box-item">2</div>
                        <div class="box-item">3</div>
                        <div class="box-item">4</div>
                    </div>
                </div>
                <div class="item">
                    <p>space-between：两端对齐，项目之间的间隔都相等。</p>
                    <div class="box box-9">
                        <div class="box-item">1</div>
                        <div class="box-item">2</div>
                        <div class="box-item">3</div>
                        <div class="box-item">4</div>
                    </div>
                </div>
                <div class="item">
                    <p>space-around：每个项目两侧的间隔相等。所以，项目之间的间隔比项目与边框的间隔大一倍。</p>
                    <div class="box box-10">
                        <div class="box-item">1</div>
                        <div class="box-item">2</div>
                        <div class="box-item">3</div>
                        <div class="box-item">4</div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <h3>5、align-items属性</h3>
    <p>align-items属性定义项目在交叉轴上如何对齐。</p>
    <p>
        .box { align-items: flex-start | flex-end | center | baseline | stretch; }
    </p>
    <div class="tab" js-tab="4">
        <div class="tab-title">
            <a href="javascript:;" class="item item-cur">flex-start</a>
            <a href="javascript:;" class="item">flex-end</a>
            <a href="javascript:;" class="item">center</a>
            <a href="javascript:;" class="item">baseline</a>
            <a href="javascript:;" class="item">stretch</a>
        </div>
        <div class="tab-cont">
            <div class="tab-cont__wrap">
                <div class="item">
                    <p>flex-start：交叉轴的起点对齐。</p>
                    <div class="box box-11">
                        <div class="box-item">1</div>
                        <div class="box-item item-tall">2</div>
                        <div class="box-item">3</div>
                        <div class="box-item item-tall">4</div>
                    </div>
                </div>
                <div class="item">
                    <p>flex-end：交叉轴的终点对齐。</p>
                    <div class="box box-12">
                        <div class="box-item">1</div>
                        <div class="box-item item-tall">2</div>
                        <div class="box-item">3</div>
                        <div class="box-item item-tall">4</div>
                    </div>
                </div>
                <div class="item">
                    <p>center：交叉轴的中点对齐。</p>
                    <div class="box box-13">
                        <div class="box-item">1</div>
                        <div class="box-item item-tall">2</div>
                        <div class="box-item">3</div>
                        <div class="box-item item-tall">4</div>
                    </div>
                </div>
                <div class="item">
                    <p>baseline: 项目的第一行文字的基线对齐。</p>
                    <div class="box box-14 line">
                        <div class="box-item">1</div>
                        <div class="box-item item-tall">2</div>
                        <div class="box-item">3</div>
                        <div class="box-item item-tall">4</div>
                    </div>
                </div>
                <div class="item">
                    <p>stretch（默认值）：如果项目未设置高度或设为auto，将占满整个容器的高度。</p>
                    <div class="box box-15">
                        <div class="box-item">1</div>
                        <div class="box-item item-tall">2</div>
                        <div class="box-item">3</div>
                        <div class="box-item item-tall">4</div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <h3>6、align-content属性</h3>
    <p>align-content属性定义了多根轴线（多行）的对齐方式。如果项目只有一根轴线，该属性不起作用。</p>
    <p>
        .box { align-content: flex-start | flex-end | center | space-between | space-around | stretch; }
    </p>
    <div class="tab" js-tab="5">
        <div class="tab-title">
            <a href="javascript:;" class="item item-cur">flex-start</a>
            <a href="javascript:;" class="item">flex-end</a>
            <a href="javascript:;" class="item">center</a>
            <a href="javascript:;" class="item">space-between</a>
            <a href="javascript:;" class="item">space-around</a>
            <a href="javascript:;" class="item">stretch</a>
        </div>
        <div class="tab-cont">
            <div class="tab-cont__wrap">
                <div class="item">
                    <p>flex-start：交叉轴的起点对齐。</p>
                    <div class="box box-tall box-16">
                        <div class="box-item">1</div>
                        <div class="box-item">2</div>
                        <div class="box-item">3</div>
                        <div class="box-item">4</div>
                        <div class="box-item">5</div>
                        <div class="box-item">6</div>
                        <div class="box-item">7</div>
                        <div class="box-item">8</div>
                        <div class="box-item">9</div>
                    </div>
                </div>
                <div class="item">
                    <p>flex-end：与交叉轴的终点对齐。</p>
                    <div class="box box-tall box-17">
                        <div class="box-item">1</div>
                        <div class="box-item">2</div>
                        <div class="box-item">3</div>
                        <div class="box-item">4</div>
                        <div class="box-item">5</div>
                        <div class="box-item">6</div>
                        <div class="box-item">7</div>
                        <div class="box-item">8</div>
                        <div class="box-item">9</div>
                    </div>
                </div>
                <div class="item">
                    <p>center：与交叉轴的中点对齐。</p>
                    <div class="box box-tall box-18">
                        <div class="box-item">1</div>
                        <div class="box-item">2</div>
                        <div class="box-item">3</div>
                        <div class="box-item">4</div>
                        <div class="box-item">5</div>
                        <div class="box-item">6</div>
                        <div class="box-item">7</div>
                        <div class="box-item">8</div>
                        <div class="box-item">9</div>
                    </div>
                </div>
                <div class="item">
                    <p>space-between：与交叉轴两端对齐，轴线之间的间隔平均分布。</p>
                    <div class="box box-tall box-19">
                        <div class="box-item">1</div>
                        <div class="box-item">2</div>
                        <div class="box-item">3</div>
                        <div class="box-item">4</div>
                        <div class="box-item">5</div>
                        <div class="box-item">6</div>
                        <div class="box-item">7</div>
                        <div class="box-item">8</div>
                        <div class="box-item">9</div>
                    </div>
                </div>
                <div class="item">
                    <p>space-around：每根轴线两侧的间隔都相等。所以，轴线之间的间隔比轴线与边框的间隔大一倍。</p>
                    <div class="box box-tall box-20">
                        <div class="box-item">1</div>
                        <div class="box-item">2</div>
                        <div class="box-item">3</div>
                        <div class="box-item">4</div>
                        <div class="box-item">5</div>
                        <div class="box-item">6</div>
                        <div class="box-item">7</div>
                        <div class="box-item">8</div>
                        <div class="box-item">9</div>
                    </div>
                </div>
                <div class="item">
                    <p>stretch（默认值）：轴线占满整个交叉轴。</p>
                    <div class="box box-tall box-21">
                        <div class="box-item">1</div>
                        <div class="box-item">2</div>
                        <div class="box-item">3</div>
                        <div class="box-item">4</div>
                        <div class="box-item">5</div>
                        <div class="box-item">6</div>
                        <div class="box-item">7</div>
                        <div class="box-item">8</div>
                        <div class="box-item">9</div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <h2>项目的属性</h2>
    <h3>1、order属性</h3>
    <p>order属性定义项目的排列顺序。数值越小，排列越靠前，默认为0。</p>
    <p>
        .item { order: &lt;integer&gt;; }
    </p>
    <div class="box box-22">
        <div class="box-item">1</div>
        <div class="box-item">2</div>
        <div class="box-item">3</div>
        <div class="box-item order">4
            <div>(order:-1)</div>
        </div>
    </div>
    <h3>2、flex-grow属性</h3>
    <p>flex-grow属性定义项目的放大比例，默认为0，即如果存在剩余空间，也不放大。</p>
    <p>如果所有项目的flex-grow属性都为1，则它们将等分剩余空间（如果有的话）。如果一个项目的flex-grow属性为2，其他项目都为1，则前者占据的剩余空间将比其他项多一倍。</p>
    <p>
        .item { flex-grow: &lt;number&gt;; /* default 0 */ }
    </p>
    <div class="box box-23">
        <div class="box-item grow">1
            <div>flex-grow: 1</div>
        </div>
        <div class="box-item grow grow-2">2
            <div>flex-grow: 2</div>
        </div>
        <div class="box-item grow">3
            <div>flex-grow: 1</div>
        </div>
    </div>
    <h3>3、flex-shrink</h3>
    <p>flex-shrink属性定义了项目的缩小比例，默认为1，即如果空间不足，该项目将缩小。</p>
    <p>如果所有项目的flex-shrink属性都为1，当空间不足时，都将等比例缩小。如果一个项目的flex-shrink属性为0，其他项目都为1，则空间不足时，前者不缩小。
        <br>负值对该属性无效。</p>
    <p>
        .item { flex-shrink: &lt;number&gt;; /* default 1 */ }
    </p>
    <div class="box box-24">
        <div class="box-item shrink">1
            <div>flex-shrink: 0</div>
        </div>
        <div class="box-item">2</div>
        <div class="box-item">3</div>
    </div>
    <h3>4、flex-basis属性</h3>
    <p>flex-basis属性定义了在分配多余空间之前，项目占据的主轴空间（main size）。浏览器根据这个属性，计算主轴是否有多余空间。它的默认值为auto，即项目的本来大小。</p>
    <p>
        .item { flex-basis: &lt;length&gt;; | auto; /* default auto */ }
    </p>
    <div class="box box-25">
        <div class="box-item">1</div>
        <div class="box-item">2</div>
        <div class="box-item">3</div>
    </div>
    <h3>5、flex属性</h3>
    <p>flex属性是flex-grow, flex-shrink 和 flex-basis的简写，默认值为0 1 auto。后两个属性可选。</p>
    <p>该属性有两个快捷值：auto (1 1 auto) 和 none (0 0 auto)。</p>
    <p>
        .item { flex: none | [ &lt;'flex-grow'&gt; &lt;'flex-shrink'&gt;? || &lt;'flex-basis'&gt; ] }
    </p>
    <h3>6、align-self属性</h3>
    <p>align-self属性允许单个项目有与其他项目不一样的对齐方式，可覆盖align-items属性。默认值为auto，表示继承父元素的align-items属性，如果没有父元素，则等同于stretch。</p>
    <p>
        .item { align-self: auto | flex-start | flex-end | center | baseline | stretch; }
    </p>
    <div class="box box-26">
        <div class="box-item">1</div>
        <div class="box-item">2</div>
        <div class="box-item end">3
            <div>flex-end</div>
        </div>
        <div class="box-item">4</div>
    </div>
    <h2>进阶实例</h2>
    <h3>一、骰子的布局</h3>
    <div class="tab" js-tab="6">
        <div class="tab-title">
            <a href="javascript:;" class="item item-cur">一个点</a>
            <a href="javascript:;" class="item">两个点</a>
            <a href="javascript:;" class="item">三个点</a>
            <a href="javascript:;" class="item">四个点</a>
            <a href="javascript:;" class="item">五个点</a>
            <a href="javascript:;" class="item">六个点</a>
        </div>
        <div class="tab-cont">
            <div class="tab-cont__wrap">
                <div class="item">
                    <div class="first-face">
                        <span class="pip"></span>
                    </div>
                    <p>
                        &lt;div class="first-face">
                        <br> &nbsp;&nbsp;&lt;span class="pip">&lt;/span>
                        <br> &lt;/div>
                    </p>
                    <p>
                        .first-face {
                        <br> &nbsp;&nbsp;display: flex;
                        <br> &nbsp;&nbsp;justify-content: center;
                        <br> &nbsp;&nbsp;align-items: center;
                        <br> }
                    </p>
                </div>
                <div class="item">
                    <div class="second-face">
                        <span class="pip"></span>
                        <span class="pip"></span>
                    </div>
                    <p>
                        &lt;div class="second-face">
                        <br> &nbsp;&nbsp;&lt;span class="pip">&lt;/span>
                        <br> &nbsp;&nbsp;&lt;span class="pip">&lt;/span>
                        <br> &lt;/div>
                    </p>
                    <p>
                        .second-face {
                        <br> &nbsp;&nbsp;display: flex;
                        <br> &nbsp;&nbsp;justify-content: space-between;
                        <br> }
                        <br> .second-face .pip:nth-of-type(2) {
                        <br> &nbsp;&nbsp;align-self: flex-end;
                        <br> }
                    </p>
                </div>
                <div class="item">
                    <div class="third-face">
                        <span class="pip"></span>
                        <span class="pip"></span>
                        <span class="pip"></span>
                    </div>
                    <p>
                        &lt;div class="third-face">
                        <br> &nbsp;&nbsp;&lt;span class="pip">&lt;/span>
                        <br> &nbsp;&nbsp;&lt;span class="pip">&lt;/span>
                        <br> &nbsp;&nbsp;&lt;span class="pip">&lt;/span>
                        <br> &lt;/div>
                    </p>
                    <p>
                        .third-face {
                        <br> &nbsp;&nbsp;display: flex;
                        <br> &nbsp;&nbsp;justify-content: space-between;
                        <br> }
                        <br> .third-face .pip:nth-of-type(2) {
                        <br> &nbsp;&nbsp;align-self: center;
                        <br> }
                        <br> .third-face .pip:nth-of-type(3) {
                        <br> align-self: flex-end;
                        <br> }
                    </p>
                </div>
                <div class="item">
                    <div class="fourth-face">
                        <div class="column">
                            <span class="pip"></span>
                            <span class="pip"></span>
                        </div>
                        <div class="column">
                            <span class="pip"></span>
                            <span class="pip"></span>
                        </div>
                    </div>
                    <p>
                        &lt;div class="fourth-face">
                        <br> &nbsp;&nbsp;&lt;div class="column">
                        <br> &nbsp;&nbsp;&nbsp;&nbsp;&lt;span class="pip">&lt;/span>
                        <br> &nbsp;&nbsp;&nbsp;&nbsp;&lt;span class="pip">&lt;/span>
                        <br> &nbsp;&nbsp;&lt;/div>
                        <br> &nbsp;&nbsp;&lt;div class="column">
                        <br> &nbsp;&nbsp;&nbsp;&nbsp;&lt;span class="pip">&lt;/span>
                        <br> &nbsp;&nbsp;&nbsp;&nbsp;&lt;span class="pip">&lt;/span>
                        <br> &nbsp;&nbsp;&lt;/div>
                        <br> &lt;/div>
                    </p>
                    <p>
                        .fourth-face{
                        <br> &nbsp;&nbsp;display: flex;
                        <br> &nbsp;&nbsp;justify-content: space-between;
                        <br> }
                        <br> .fourth-face .column{
                        <br> &nbsp;&nbsp;display: flex;
                        <br> &nbsp;&nbsp;flex-direction: column;
                        <br> &nbsp;&nbsp;justify-content: space-between;
                        <br> }
                    </p>
                </div>
                <div class="item">
                    <div class="fifth-face">
                        <div class="column">
                            <span class="pip"></span>
                            <span class="pip"></span>
                        </div>
                        <div class="column">
                            <span class="pip"></span>
                        </div>
                        <div class="column">
                            <span class="pip"></span>
                            <span class="pip"></span>
                        </div>
                    </div>
                    <p>
                        &lt;div class="fifth-face">
                        <br> &nbsp;&nbsp;&lt;div class="column">
                        <br> &nbsp;&nbsp;&nbsp;&nbsp;&lt;span class="pip">&lt;/span>
                        <br> &nbsp;&nbsp;&nbsp;&nbsp;&lt;span class="pip">&lt;/span>
                        <br> &nbsp;&nbsp;&lt;/div>
                        <br> &nbsp;&nbsp;&lt;div class="column">
                        <br> &nbsp;&nbsp;&nbsp;&nbsp;&lt;span class="pip">&lt;/span>
                        <br> &nbsp;&nbsp;&lt;/div>
                        <br> &nbsp;&nbsp;&lt;div class="column">
                        <br> &nbsp;&nbsp;&nbsp;&nbsp;&lt;span class="pip">&lt;/span>
                        <br> &nbsp;&nbsp;&nbsp;&nbsp;&lt;span class="pip">&lt;/span>
                        <br> &nbsp;&nbsp;&lt;/div>
                        <br> &lt;/div>
                    </p>
                    <p>
                        .fifth-face {
                        <br> &nbsp;&nbsp;display: flex;
                        <br> &nbsp;&nbsp;justify-content: space-between;
                        <br> }
                        <br> .fifth-face .column {
                        <br> &nbsp;&nbsp;display: flex;
                        <br> &nbsp;&nbsp;flex-direction: column;
                        <br> &nbsp;&nbsp;justify-content: space-between;
                        <br> }
                        <br> .fifth-face .column:nth-of-type(2) {
                        <br> &nbsp;&nbsp;justify-content: center;
                        <br> }
                    </p>
                </div>
                <div class="item">
                    <div class="sixth-face">
                        <div class="column">
                            <span class="pip"></span>
                            <span class="pip"></span>
                            <span class="pip"></span>
                        </div>
                        <div class="column">
                            <span class="pip"></span>
                            <span class="pip"></span>
                            <span class="pip"></span>
                        </div>
                    </div>
                    <p>
                        &lt;div class="sixth-face">
                        <br> &nbsp;&nbsp;&lt;div class="column">
                        <br> &nbsp;&nbsp;&nbsp;&nbsp;&lt;span class="pip">&lt;/span>
                        <br> &nbsp;&nbsp;&nbsp;&nbsp;&lt;span class="pip">&lt;/span>
                        <br> &nbsp;&nbsp;&nbsp;&nbsp;&lt;span class="pip">&lt;/span>
                        <br> &nbsp;&nbsp;&lt;/div>
                        <br> &nbsp;&nbsp;&lt;div class="column">
                        <br> &nbsp;&nbsp;&nbsp;&nbsp;&lt;span class="pip">&lt;/span>
                        <br> &nbsp;&nbsp;&nbsp;&nbsp;&lt;span class="pip">&lt;/span>
                        <br> &nbsp;&nbsp;&nbsp;&nbsp;&lt;span class="pip">&lt;/span>
                        <br> &nbsp;&nbsp;&lt;/div> &lt;/div>
                    </p>
                    <p>
                        .sixth-face{
                        <br> &nbsp;&nbsp;display: flex;
                        <br> &nbsp;&nbsp;justify-content: space-between;
                        <br> }
                        <br> .sixth-face .column{
                        <br> &nbsp;&nbsp;display: flex;
                        <br> &nbsp;&nbsp;flex-direction: column;
                        <br> &nbsp;&nbsp;justify-content: space-between;
                        <br> }
                    </p>
                </div>
            </div>
        </div>
    </div>
    <h3>二、网格布局</h3>
    <h4>2.1 基本网格布局</h4>
    <!-- <img src="image/grid1.png" alt=""> -->
    <div class="Grid">
        <div class="Grid-cell">1/2</div>
        <div class="Grid-cell">1/2</div>
    </div>
    <div class="Grid">
        <div class="Grid-cell">1/3</div>
        <div class="Grid-cell">1/3</div>
        <div class="Grid-cell">1/3</div>
    </div>
    <div class="Grid">
        <div class="Grid-cell">1/4</div>
        <div class="Grid-cell">1/4</div>
        <div class="Grid-cell">1/4</div>
        <div class="Grid-cell">1/4</div>
    </div>
    <textarea name="" id="" cols="60" rows="10" disabled="true">
        <div class="Grid">
            <div class="Grid-cell">1/3</div>
            <div class="Grid-cell">1/3</div>
            <div class="Grid-cell">1/3</div>
        </div>
    </textarea>
    <textarea name="" id="" cols="60" rows="10" disabled="true">
        .Grid { display: flex; } .Grid-cell { flex: 1; }
    </textarea>
    <h4>2.2 百分比布局</h4>
    <!-- <img src="image/grid2.png" alt=""> -->
    <div class="Grid">
        <div class="Grid-cell u-1of2">1/2</div>
        <div class="Grid-cell">auto</div>
        <div class="Grid-cell">auto</div>
    </div>
    <div class="Grid">
        <div class="Grid-cell">auto</div>
        <div class="Grid-cell u-1of3">1/3</div>
    </div>
    <div class="Grid">
        <div class="Grid-cell u-1of4">1/4</div>
        <div class="Grid-cell">auto</div>
        <div class="Grid-cell u-1of3">1/3</div>
    </div>
    <textarea name="" id="" cols="60" rows="20" disabled="true">
        <div class="Grid">
            <div class="Grid-cell u-1of2">1/2</div>
            <div class="Grid-cell">auto</div>
            <div class="Grid-cell">auto</div>
        </div>
        <div class="Grid">
            <div class="Grid-cell">auto</div>
            <div class="Grid-cell u-1of3">1/3</div>
        </div>
        <div class="Grid">
            <div class="Grid-cell u-1of4">1/4</div>
            <div class="Grid-cell">auto</div>
            <div class="Grid-cell u-1of3">1/3</div>
        </div>
    </textarea>
    <textarea name="" id="" cols="60" rows="20" disabled="true">
        .Grid { display: flex; } .Grid-cell { flex: 1; } .Grid-cell.u-full { flex: 0 0 100%; } .Grid-cell.u-1of2 { flex: 0 0 50%; } .Grid-cell.u-1of3 { flex: 0 0 33.3333%; } .Grid-cell.u-1of4 { flex: 0 0 25%; }
    </textarea>
    <h3>三、圣杯布局</h3>
    <p>圣杯布局（Holy Grail Layout）指的是一种最常见的网站布局。页面从上到下，分成三个部分：头部（header），躯干（body），尾部（footer）。其中躯干又水平分成三栏，从左到右为：导航、主栏、副栏。</p>
    <img src="image/holygrid.png" alt="">
    <textarea name="" id="" cols="50" rows="20" disabled="true">
<body class="HolyGrail">
    <header>...</header>
    <div class="HolyGrail-body">
        <main class="HolyGrail-content">...</main>
        <nav class="HolyGrail-nav">...</nav>
         <aside class="HolyGrail-ads">...</aside>
    </div>
    <footer>...</footer>
</body>
    </textarea>
    <textarea name="" id="" cols="60" rows="22" disabled="true">
.HolyGrail {
  display: flex;
  min-height: 100vh;
  flex-direction: column;
}
header,footer {
  flex: 1;
}
.HolyGrail-body {
  display: flex;
  flex: 1;
}
.HolyGrail-content {
  flex: 1;
}
.HolyGrail-nav, .HolyGrail-ads {
  flex: 0 0 12em;  /* 两个边栏的宽度设为12em */
}
.HolyGrail-nav {
  order: -1;  /* 导航放到最左边 */
}
    </textarea>
    <textarea name="" id="" cols="60" rows="22" disabled="">
 @media (max-width: 768px) {
    .HolyGrail-body {
      flex-direction: column;
      flex: 1;
    }
    .HolyGrail-nav,
    .HolyGrail-ads,
    .HolyGrail-content {
      flex: auto;
    }
}
<!-- 如果是小屏幕，躯干的三栏自动变为垂直叠加 -->
    </textarea>
    <h3>四、流式布局</h3>
    <p>每行的项目数固定，会自动分行。</p>
    <div class="contain">
    <img src="image/flow.png" alt="">
    <textarea name="" id="" cols="60" rows="30">
	.parent {
  		width: 200px;
  		height: 150px;
  		background-color: black;
  		display: flex;
  		flex-flow: row wrap;
  		align-content: flex-start;
	}

	.child {
  		box-sizing: border-box;
  		background-color: white;
  		flex: 0 0 25%;
  		height: 50px;
  		border: 1px solid red;
	}
    </textarea>
    </div>
    <script src="js/jquery-1.8.3.min.js"></script>
    <script src="js/tab.js"></script>
    <script>
    $(function() {
        $('[js-tab=1]').tab();
        $('[js-tab=2]').tab();
        $('[js-tab=3]').tab();
        $('[js-tab=4]').tab();
        $('[js-tab=5]').tab();
        $('[js-tab=6]').tab();
    });
    </script>
</body>

</html>
