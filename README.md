# User Interface Specification Document

## Global Components UI<br/>

#### Page style properties:<br/>
<ul>
    <li>Page body background-color: #fff</li>
    <li>main-color: #007cba (all button background-color and table head background-color...etc)</li>
</ul>

#### Top-bar style properties:<br/>
<ul>
    <li>background-color: #f5f5f5</li>
    <li>The height of the top-bar is 40px.</li>
</ul>

#### Button component style properties:<br/>
<ul>
    <li>The background color must be the main color defined in the "Page Style".</li>
    <li>height: 24px</li>
    <li>border: 1px solid #006dad</li>
    <li>font color: #fff</li>
    <li>padding: 8px 10px</li>
    <li>line-height: 24px (So that the position of the text is in the middle, if you have any other solution you can use.)</li>
    <li>What will happen if it gets an attributes called 'disabled'
        <ul>
            <li>Opacity should be set to '0.8'.</li>
        </ul>
    </li>
</ul>

---

## First Page UI<br/>

When the page is first opened, a screen will appear listing the users.<br/>

First there should be a "top-bar" at the top of the page.<br/>

#### Components to be used in the topbar and their properties<br/>

<ul>
    <li>Button component:
        <ul>
            <li>'Button Component' properties defined above will be used.</li>
            <li>Left margin must be 20px</li>
            <li>Button icon: Plus Icon</li>
            <li>Button text: New User</li>
            <li>If there is a click event, it should switch to the new-user page</li>
        </ul>
    </li>
    <li>Topbar checkbox component:
        <ul>
            <li>Checkbox label text: "Hide Disabled User"</li>
            <li>Hide disabled users if checkbox is selected.(if enabled=false)</li>
            <li>The label should be to the right of the checkbox and have a distance of 2px between them.</li>
        </ul>
    </li>
</ul>



#### Components to be used in the content and their properties:<br/>
<ul>
    <li>There should be 4 columns.
        <ul>
            <li>ID</li>
            <li>User Name</li>
            <li>Email</li>
            <li>Enabled</li>
        </ul>
    </li>
    <li>It should cover the entire width of the page.</li>
    <li>Each column should have a filter icon in its header.</li>
    <li>When the header in each column is clicked, there should be 3 options and you should give an icon accordingly.
        <ul>
            <li>ASC(ascendant)</li>
            <li>DESC(descendant)</li>
            <li>By creation time</li>
        </ul>
    </li>
    <li>Each column will have a border-right: #ededed.</li>
    <li>Font color must be #000.</li>
    <li>The background color must be the main color defined in the "Page Style".</li>
    <li>If any line hover the background color is: #b9d9e8</li>
</ul>

Clicking on the "new user" button will redirect to the "new user" page.

---

## New User Page UI<br/>

#### Topbar page design

<ul>
    <li>Button component:
        <ul>
            <li>'Button Component' properties defined above will be used.</li>
            <li>Align right.</li>
            <li>Right margin must be 20px</li>
            <li>Button text: Save User</li>
            <li>The following inputs will get the disabled attribute unless populated and the select box is not selected.</li>
        </ul>
    </li>
</ul>

#### Input component style properties:
<ul>
    <li>Label style:
        <ul>
            <li>font color: #000</li>
            <li>width: 100px</li>
        </ul>
    </li>
    <li>Input style:
        <ul>
            <li>height: 24px</li>
            <li>border: 2px solid #d9d9d9</li>
            <li>font color: #000</li>
        </ul>
    </li>
    <li>Labels and inputs will be side by side.("display: flex;" It is recommended to use. For responsive, "flex-direction:column;" can be used on small screens.)</li>
</ul>

#### Content page design
<ul>
    <li>Title style:
        <ul>
            <li>background-color: #f5f5f5</li>
            <li>height: 42px</li>
            <li>line-height: 42px</li>
            <li>font-size: 22px</li>
            <li>padding-left: 15px</li>
        </ul>
    </li>
    <li>Username input style:
        <ul>
            <li>It is using the above input component properties.</li>
            <li>Label text: 'Username: '</li>
        </ul>
    </li>
    <li>Display name input style:
        <ul>
            <li>It is using the above input component properties.</li>
            <li>Label text: 'Display Name: '</li>
        </ul>
    </li>
    <li>Phone input style:
        <ul>
            <li>It is using the above input component properties.</li>
            <li>Label text: 'Phone: '</li>
        </ul>
    </li>
    <li>Email input style:
        <ul>
            <li>It is using the above input component properties.</li>
            <li>Label text: 'Email: '</li>
        </ul>
    </li>
    <li>User roles selectbox style:
        <ul>
            <li>Label style:
                <ul>
                    <li>font color: #000</li>
                    <li>width: 100px</li>
                </ul>
            </li>
            <li>Label Text: 'User Roles: '</li>
            <li>Selectbox style:
                <ul>
                    <li>height: 24px</li>
                    <li>border: 2px solid #d9d9d9</li>
                    <li>font color: #90919c</li>
                </ul>
            </li>
            <li>Label and checkbox will be side by side.("display: flex;" It is recommended to use. For responsive, "flex-direction:column;" can be used on small screens.)</li>
            <li>Options to be given in the select box:
                <ul>
                    <li>Guest</li>
                    <li>Admin</li>
                    <li>SuperAdmin</li>
                </ul>
            </li>
            <li>If there is no selection text = 'Select user roles...'</li>
        </ul>
    </li>
    <li>Checkbox style
        <ul>
            <li>Label style:
                <ul>
                    <li>font color: #000</li>
                    <li>width: 100px</li>
                </ul>
            </li>
            <li>Label Text: Enabled</li>
            <li>Label and checkbox will be side by side.("display: flex;" It is recommended to use. For responsive, "flex-direction:column;" can be used on small screens.)</li>
        </ul>
    </li>
</ul>

When the save user button is clicked, the save process will take place. After registering it will take you back to the first page.