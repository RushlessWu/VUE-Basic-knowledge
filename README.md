* Vue.js��ʲô?			
	"*�����ǰ��������Ϫ,ǰ�ȸ�ǰ�˹���ʦ"		
"  * ��angular.js���Ƶ�������ʽ�����������ܸ���angular�����С�ܶ�, �Ƚ��ʺ��ƶ��˿���"			
"  * ��������ȫ�ܿ��, ֻ��עUI, �����Ҫrouter/ajax, ����ʹ�ö�Ӧ�����ʹ�ñ�Ŀ���ʵ��"			
  			
* ����ʹ��			
	* ����vue.js		
	"* ����Vue����, ָ��ѡ�����"		
		* el : ָ��dom��ǩ������ѡ����	
		* data : ָ����ʼ��״̬�������ݵĶ���	
		        ����/����(����һ������)	
	* ҳ����		
		* ʹ��v-model: ʵ��˫�����ݰ�	
		* ʹ��{{}}: ��ʾ����	
			
* Vue�����ѡ��			
	* el		
	  * ָ��dom��ǩ������ѡ����		
		* Vue�ͻ�����Ӧ�ı�ǩ�����ӱ�ǩ	
	* data		
		* ָ����ʼ��״̬�������ݵĶ���	
		* vue�������ֱ�ӷ���������	
		* ҳ���п���ֱ�ӷ���ʹ��	
	* methods		
		* ������������Ķ���	
		* ��ҳ���е��¼�ָ�����󶨻ص�	
		"* �ص�����Ĭ����event����, ��Ҳ����ָ���Լ��Ĳ���"	
		"* ���еķ�����vue����������, ����data�е�����ֱ��ʹ��this.xxx"	
	* computed		
		* ������������Ķ���	
		"* ��״̬���Խ��м��㷵��һ���µ�����, ��ҳ���ȡ��ʾ"	
		* һ����������൱����һ��ֻ��������	
		"* ����set/get������ʵ���������ݵļ����ȡ, ͬʱ�����������ݵı仯"	
	* watch		
		* ����������Լ��ӵĶ���	
		* ��Ϊһ����Ӻ���ȼ���	
      ```			
      'xxx' : {			
"        deep : true,"			
        handler : fun(value)			
      }			
      ```			
			
* ��չ����			
  * ������ĳ��÷��������˰�װ(�������ݰ�)			
	* $remove(item) : ɾ�������ж�Ӧ��Ԫ��		
	"* $set(index, ele) : ��������ָ���±�ָ����Ӧ��Ԫ�� "		
			
* vue����������			
  * 			
			
			
* ҳ��ָ��			
	* v-text/v-html: ָ����ǩ��		
    * v-text : �������ı�			
		* v-html : ��value��Ϊhtml��ǩ������	
	* v-if v-else v-show		
		"* v-if : ���vlaueΪtrue, ��ǰ��ǩ�������ҳ����"	
		"* v-else : ��v-ifһ��ʹ��, ���valueΪfalse, ����ǰ��ǩ�����ҳ����"	
		"* v-show: �ͻ��ڱ�ǩ�����display��ʽ, ���vlaueΪtrue, display=block, ������none"	
	* v-for : ����		
		* �������� : v-for="person in persons"   $index	
		* �������� : v-for="value in person"   $key	
	* v-on : ���¼�����		
		"* v-on:�¼���, ������дΪ: @�¼���"	
		* ���Ӿ���İ���: @keyup.keyCode   @keyup.enter	
		* ��ֹ�¼���ð�ݺ��¼�Ĭ����Ϊ: @click.stop   @click.prevent	
		* ��������: $event	
	* v-bind : ǿ�ư󶨽������ʽ  		
		"* �ܶ�����ֵ�ǲ�֧�ֱ��ʽ��, �Ϳ���ʹ��v-bind"	
		* ������дΪ:  :id='nanme'	
		* :class	
		  * :class="a"	
			"* :class=""{classA : isA, classB : isB}"""
			"* :class=""[classA, classB]"""
		* :style	
			:style="{color : color}"
	* v-model		
		* ˫�����ݰ�	
	* v-el : ��ʶĳ����ǩ		
		* v-el:xxx	
		* ��ȡ�õ���ǩ����: this.$els.xxx	
			
* ������			
  * ����			
    * capitalize : ����ĸ��С			
    * uppercase : ȫ����д			
    * lowercase : ȫ��Сд			
    * currency : ���һ�			
    * pluralize : ����/��������			
    * json : json��ʽ��			
			
    * limitBy : �޶�����Ĳ���Ԫ��(�±�)			
    * filterBy : �޶�����Ĳ���Ԫ��(ֵ)			
    * orderBy : �������������			
  * �Զ���			
  * ȫ�ֹ�����			
    ```			
"    Vue.filter('��������', function(value, xxx, yyy) {"			
      //�����߼�			
      return result;			
    })			
    ```			
  * �ֲ�������			
    ```			
    new Vue({			
      filters : {			
"        '��������' : function(value, xxx, yyy) {"			
            //�����߼�			
            return result;			
        }			
      }			
    })			
    ```			
* ָ��			
  * ����			
    * v:text : ����Ԫ�ص� textContent			
    * v-html : ����Ԫ�ص� innerHTML			
"    * v-if : ���Ϊtrue, ��ǰ��ǩ�Ż������ҳ��"			
"    * v-else: ���Ϊfalse, ��ǰ��ǩ�Ż������ҳ��"			
    * v-show : ͨ������display��ʽ��������ʾ/����			
    * v-for : ��������/����			
"    * v-on : ���¼�����, һ���дΪ@"			
"    * v-bind : ǿ�ư󶨽������ʽ, ����ʡ��v-bind"			
    * v-model : ˫�����ݰ�			
"    * v-el : Ϊĳ��Ԫ��ע��һ��Ψһ��ʶ, vue����ͨ��$els���Է������Ԫ�ض���"			
"    * v-cloak : ʹ������ֹ���ֱ��ʽ, ��css���: [v-cloak] { display: none }"			
  * �Զ���			
    * ע��ȫ��ָ��			
      ```			
"      Vue.directive('my-directive', function(value){"			
        this.el.innerHTML = value.toUpperCase();			
      })			
      ```			
    * ע��ֲ�ָ��			
      ```			
      directives : {			
        'my-directive' : function(value) {			
          this.el.innerHTML = value;			
        }			
      }			
      ```			
