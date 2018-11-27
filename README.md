EverFramework Help
==================

사용된 기술
----------

1. Custom Tag Library
2. Google Closure Template
3. Open javascript libraries (jQuery, jQueryUI, BootStrap, etc.)
4. Spring MVC Framework
5. RealGrid

커스텀태그 구조
--------------
```html
<e:ui>
    <script type="text/javascript">...</script>
    <e:ui>
        <e:searchPanel ...>
            <e:row>
                <e:label ... />
                <e:field ...>
                    <e:inputText .../>
                </e:field>
                <e:label ... />
                <e:field ...>
                    <e:inputText .../>
                </e:field>
            </e:row>
        </e:searchPanel>
        <e:buttonBar ...>
            <e:button .../>
        </e:buttonBar>
        <e:gridPanel .../>
    </e:ui>
</e:ui>
```

UI 구조 및 상속
--------------

AbstractObject ← AbstractComponent ← AbstractEditField, AbstractContainer

AbstractEditField ← InputText, InputDate, InputPassword, InputHidden, Search

AbstractContainer ← Window, SearchPanel, ButtonBar, Panel


- AbstractEditField
