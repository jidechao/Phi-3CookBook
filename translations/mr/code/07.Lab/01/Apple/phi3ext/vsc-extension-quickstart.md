# तुमच्या VS Code विस्तारामध्ये स्वागत आहे

## या फोल्डरमध्ये काय आहे

* या फोल्डरमध्ये तुमच्या विस्तारासाठी आवश्यक असलेल्या सर्व फाइल्स आहेत.
* `package.json` - हे मॅनिफेस्ट फाइल आहे, ज्यामध्ये तुम्ही तुमच्या विस्ताराची आणि कमांडची घोषणा करता.
  * उदाहरणासाठी दिलेला प्लगइन एक कमांड नोंदवतो आणि त्याचे शीर्षक व कमांडचे नाव परिभाषित करतो. या माहितीच्या आधारे VS Code कमांड पॅलेटमध्ये कमांड दाखवू शकतो. सध्या प्लगइन लोड करण्याची आवश्यकता नाही.
* `src/extension.ts` - हे मुख्य फाइल आहे जिथे तुम्ही तुमच्या कमांडची अंमलबजावणी पुरवता.
  * फाइल एक फंक्शन निर्यात करते, `activate`, जेव्हा तुमचा विस्तार प्रथमच सक्रिय केला जातो (या प्रकरणात कमांड चालवून). `activate` फंक्शनमध्ये आपण `registerCommand` कॉल करतो.
  * आम्ही कमांडची अंमलबजावणी असलेले फंक्शन `registerCommand` ला दुसऱ्या पॅरामीटर म्हणून पाठवतो.

## सेटअप

* शिफारस केलेल्या विस्तारांना स्थापित करा (amodio.tsl-problem-matcher, ms-vscode.extension-test-runner, आणि dbaeumer.vscode-eslint).

## लगेच सुरुवात करा

* तुमचा विस्तार लोड केलेल्या नवीन विंडोमध्ये उघडण्यासाठी `F5` दाबा.
* कमांड पॅलेटमधून तुमचा कमांड चालवा (`Ctrl+Shift+P` किंवा Mac साठी `Cmd+Shift+P` दाबून) आणि `Hello World` टाइप करा.
* तुमच्या विस्ताराचे डिबग करण्यासाठी `src/extension.ts` मधील कोडमध्ये ब्रेकपॉइंट सेट करा.
* डिबग कन्सोलमध्ये तुमच्या विस्ताराचा आउटपुट शोधा.

## बदल करा

* `src/extension.ts` मधील कोड बदलल्यानंतर डिबग टूलबारमधून विस्तार पुन्हा सुरू करू शकता.
* तुमच्या विस्ताराचे बदल लोड करण्यासाठी VS Code विंडो पुन्हा लोड (`Ctrl+R` किंवा Mac साठी `Cmd+R`) करू शकता.

## API शोधा

* तुम्ही फाइल `node_modules/@types/vscode/index.d.ts` उघडल्यावर आमच्या API चा पूर्ण संच पाहू शकता.

## चाचण्या चालवा

* [Extension Test Runner](https://marketplace.visualstudio.com/items?itemName=ms-vscode.extension-test-runner) स्थापित करा.
* **Tasks: Run Task** कमांडद्वारे "watch" टास्क चालवा. हे चालू असल्याची खात्री करा, अन्यथा चाचण्या शोधल्या जाऊ शकणार नाहीत.
* अॅक्टिव्हिटी बारमधील Testing दृश्य उघडा आणि "Run Test" बटणावर क्लिक करा किंवा `Ctrl/Cmd + ; A` हा हॉटकी वापरा.
* चाचणी निकालाचे आउटपुट Test Results दृश्यामध्ये पाहा.
* `src/test/extension.test.ts` मध्ये बदल करा किंवा `test` फोल्डरमध्ये नवीन चाचणी फाइल्स तयार करा.
  * दिलेला चाचणी रनर फक्त नावाच्या नमुन्याशी जुळणाऱ्या फाइल्स विचारात घेईल `**.test.ts`.
  * तुम्ही तुमच्या चाचण्यांचे कोणत्याही प्रकारे संरचना करण्यासाठी `test` फोल्डरमध्ये फोल्डर्स तयार करू शकता.

## पुढे जा

* [तुमच्या विस्ताराचे बंडलिंग करून](https://code.visualstudio.com/api/working-with-extensions/bundling-extension) विस्ताराचा आकार कमी करा आणि सुरू होण्याचा वेळ सुधारित करा.
* तुमचा विस्तार [VS Code विस्तार मार्केटप्लेसवर प्रकाशित करा](https://code.visualstudio.com/api/working-with-extensions/publishing-extension).
* [सतत एकत्रिकरण](https://code.visualstudio.com/api/working-with-extensions/continuous-integration) सेटअप करून बांधकाम स्वयंचलित करा.

**अस्वीकरण**:  
हे दस्तऐवज मशीन-आधारित एआय भाषांतर सेवांचा वापर करून अनुवादित केले गेले आहे. आम्ही अचूकतेसाठी प्रयत्नशील असलो तरी, कृपया लक्षात घ्या की स्वयंचलित अनुवादांमध्ये त्रुटी किंवा अचूकतेचा अभाव असू शकतो. मूळ दस्तऐवज त्याच्या मूळ भाषेत अधिकृत स्रोत मानला जावा. महत्त्वाच्या माहितीसाठी, व्यावसायिक मानवी भाषांतराची शिफारस केली जाते. या भाषांतराच्या वापरामुळे उद्भवणाऱ्या कोणत्याही गैरसमज किंवा चुकीच्या अर्थ लावण्यास आम्ही जबाबदार राहणार नाही.