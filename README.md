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

UI 컴포넌트 구조 및 종류
-----------------------

1. 입력, 컨테이너 컴포넌트가 상속받는 컴포넌트

 상속 컴포넌트명                             | 설명
--------------------------------------------|----------------
AbstractObject                              | 컴포넌트 이벤트 관리
AbstractComponent extends AbstractObject    | id, name 등 전체 컴포넌트가 가지는 공통속성 및 함수 정의
AbstractEditField extends AbstractComponent | 사용자 입력 컴포넌트에 대한 공통속성 및 함수 정의
AbstractContainer extends AbstractComponent | 컴포넌트 컨테이너에 대한 공통속성 및 함수 정의

2. 입력컴포넌트 종류 및 기능

 입력 컴포넌트명                             | 설명
--------------------------------------------|----------------
InputText                                   | 텍스트를 입력받는 컴포넌트
InputDate                                   | 날짜를 선택 또는 입력받는 컴포넌트
InputNumber                                 | 숫자값만 입력받는 컴포넌트
InputPassword                               | 비밀번호를 입력받는 컴포넌트
InputHidden                                 | 서버로 특정값을 전송하기 위해 화면에서는 숨겨진 컴포넌트
Search                                      | 검색에 사용되는 컴포넌트
Radio                                       | 라디오버튼 컴포넌트
Check                                       | 체크버튼 컴포넌트
TextArea                                    | 한줄 이상의 텍스트를 입력받는 컴포넌트
RichTextEditor                              | 리치텍스트 에디터 컴포넌트

3. 컨테이너 컴포넌트 종류 및 기능

 컨테이너 컴포넌트명                          | 설명
--------------------------------------------|----------------
Window                                      | 화면이름, 특수버튼(즐겨찾기, 그리드커스터마이징 기능) 화면 표시
SearchPanel                                 | 입력컴포넌트들을 테이블로 표시
ButtonBar                                   | 버튼을 표시, 좌우정렬 등 세부조절
Panel                                       | 화면을 반으로 나누거나 할 때 사용하는 컨테이너
RadioGroup                                  | 라디오버튼 컴포넌트를 그룹화하여 사용, 체크된 값 등을 가져오는 등의 함수 정의
CheckGroup                                  | 체크버튼 컴포넌트르르 그룹화하여 사용, 체크된 값 등을 가져오는 등의 함수 정의


