//Dynamic-Tabs
//Basic code for a method that creates tabs on a JTabbedPane based on iterations

/* 						I wrote this code while I was looking for it on internet.
	 * 				Due to the fact that I found nothing similar to it, I had to make it, and I uploaded
	 * 							it so you won't have the same problem. Hope it serves you well.
	 * 				You can use this on whatever you want, as long as you give me the credit for this code. 
	 */

import javax.swing.JPanel;
import javax.swing.JTabbedPane;
import javax.swing.JTextArea;

public class Tabfiller {

	public static void main(String[] args) {
	}
  
	/*Basic method to dynamically fill a JtabbedPane. for it to fulfill its purpose, you should
	 *add it to some iteration method (while,for). In this example, it will be filled with a TextArea
	 *and the textArea will be filled with a String. The input required for it will only be an already
	 *created JTabbedPane.
	 *It's only an example, so it will be filled with really simple code. You can add whatever
	 *you need to it, and it should work flawlessly
	 */
   
	public void filler (JTabbedPane tabpane) {
		JPanel jPanel = new JPanel();
		jPanel.setLayout(null);
		JTextArea textArea = new JTextArea();
		String aux = new String ("Hello World");
		tabpane.addTab(("Tab"), null, jPanel, null);
		jPanel.add(textArea);
		textArea.setText(aux);
		aux="";
	}
}
