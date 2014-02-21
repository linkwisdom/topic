指出下面的CSS文件的不规范之处；(列出所触犯的规范及相应的函数即可)

并且将以下css调整为less格式

```css
#accountScoreTabHeaders li:hover {
    cursor: pointer;
}
#accountScoreTabHeaders li.selected:hover {
    background: none;
    cursor: default;
}
#accountScoreTabHeaders .score_tab {
    float: left;
    width: 240px;
    height: 85px;
    position: relative;
    border-top: 1px solid #F9F9F9;
    border-left: 1px solid #E5E5E5;
}
#accountScoreTabHeaders .score_tab DIV {
    float: left;
    padding: 6px;
}
#accountScoreTabHeaders .score_type_name {
    color: #909090;
}
#accountScoreTabHeaders .score_change_info {
    padding-top: 38px;
    font-size: 15px;
    color: #000000;
}
#accountScoreTabHeaders .score_state {
    font-weight: bold;
}
#accountScoreTabHeaders .good {
    color: #FB3B3C
}
#accountScoreTabHeaders .bad {
    color: #249123
}
#accountScoreTabHeaders .score_value {
    color: #646569;
    font-size:57px;
    color:#666666;
    padding-top: 3px;
}
#accountScoreTabHeaders .selected {
    border-top: 1px solid #E5E5E5;
    border-bottom: 2px solid #FFFFFF;
    margin-bottom: -2px;
}
#accountScoreTabHeaders .selected .score_type_name {
    font-weight: bold;
    color: #000000;
}
#accountScoreTabHeaders .selected .score_value {
    color: #000000;
}
#accountScoreTabHeaders .main_tab {
    border-left: none;
    border-top: none;
    width: 263px;
}
#accountScoreTabHeaders .main_tab DIV {
    margin-top: -12px;
}
#accountScoreTabHeaders .main_tab .score_value {
    font-size: 70px;
}
#accountScoreTabHeaders .main_tab .score_change_info {
    padding-top: 48px;
}
```
