# Paginations-Jinja2-Bootstrap-Templates
![paginationStyle1-Success](/images/pg2009of14915.JPG)

This is a collection bootstraped jinja 2 pagination templates.

**Use case**: [See the required two steps below](#how-to-use). For example, in a Django app or better stiil, flask app using sqlachemy may purge out query results in pages using the pagination attribute. In such cases, one of the styles here can be included in the template to take care of page numbering.

**Stlyes**: As I hope to keep adding more styles, currently, the available ones are:

1. **paginationStyle1**: within a range of ```1``` to ```n```, a given page number ```x``` is displayed as ``` 1 [...] x-1 x x+1 [...] n ```.<table>
    <th>Look</th>
    <th>Use</th>
        <tr>
            <td>1 2 ... 3000</td>
            <td>for page 1</td>
        </tr>
        <tr>
            <td>1 2 3 ... 3000</td>
            <td>for page 2</td>
        </tr>
        <tr>
            <td>1 2 3 4 ... 3000</td>
            <td>for page 3</td>
        </tr>
        <tr>
            <td>1 ... 95 96 97 ... 3000</td>
            <td>for page 96</td>
        </tr>
        <tr>
            <td>1 ... 2997 2998 2999 3000</td>
            <td>for page 2998</td>
        </tr>
        <tr>
            <td>1 ... 2998 2999 3000</td>
            <td>for page 2999</td>
        </tr>
        <tr>
            <td>1 ... 2999 3000</td>
            <td>for page 3000</td>
    </table>
    Though two colour versions of paginationStyle1 are provided here, but they can alway be changed using bootstrap clases.

    a. paginationStyle1-Success uses a green background 
    ![pg1of14915.JPG](/images/pg1of14915.JPG)  
    ![pg2of14915.JPG](/images/pg2of14915.JPG)  
    ![pg3of14915.JPG](/images/pg3of14915.JPG)  
    ![pg2009of14915.JPG](/images/pg2009of14915.JPG)  
    ![pg14913of14915.JPG](/images/pg14913of14915.JPG)  
    ![pg14914of14915.JPG](/images/pg14914of14915.JPG)  
    ![pg14915of14915.JPG](/images/pg14915of14915.JPG) 

    b. paginationStyle1-Secondary is same as paginationStyle1-Success but a grey button, this time.



## How To Use
1. include your desired style in your template, something like:
{% include paginationStyle1_Success.html %}

2. use find and replace to change the default ```entries_list``` in the paginationStylex_xxxxx.html variable to your pagination object variable name.


