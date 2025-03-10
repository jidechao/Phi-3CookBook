В контекста на Phi-3-mini, „инференция“ се отнася до процеса на използване на модела за правене на прогнози или генериране на изходи въз основа на входни данни. Нека ви предоставя повече подробности за Phi-3-mini и неговите възможности за инференция.

Phi-3-mini е част от серията модели Phi-3, пуснати от Microsoft. Тези модели са създадени, за да променят представата за възможностите на Малките Езикови Модели (SLMs).

Ето някои ключови точки относно Phi-3-mini и неговите възможности за инференция:

## **Общ преглед на Phi-3-mini:**
- Phi-3-mini има размер на параметрите от 3.8 милиарда.
- Може да работи не само на традиционни изчислителни устройства, но и на edge устройства като мобилни устройства и IoT устройства.
- Пускането на Phi-3-mini позволява на физически лица и предприятия да внедряват SLMs на различни хардуерни устройства, особено в среди с ограничени ресурси.
- Поддържа различни формати на модела, включително традиционния формат на PyTorch, квантизираната версия във формат gguf и базираната на ONNX квантизирана версия.

## **Достъп до Phi-3-mini:**
За достъп до Phi-3-mini можете да използвате [Semantic Kernel](https://github.com/microsoft/SemanticKernelCookBook?WT.mc_id=aiml-138114-kinfeylo) в Copilot приложение. Semantic Kernel е съвместим както с Azure OpenAI Service, така и с отворените модели на Hugging Face и локални модели.  
Можете също така да използвате [Ollama](https://ollama.com) или [LlamaEdge](https://llamaedge.com) за извикване на квантизирани модели. Ollama позволява на отделни потребители да извикват различни квантизирани модели, докато LlamaEdge предоставя междуплатформена достъпност за GGUF модели.

## **Квантизирани модели:**
Много потребители предпочитат да използват квантизирани модели за локална инференция. Например, можете директно да стартирате Ollama с Phi-3 или да го конфигурирате офлайн, използвайки Modelfile. Modelfile определя пътя до GGUF файла и формата на подканата.

## **Възможности за Генеративен AI:**
Комбинирането на SLMs като Phi-3-mini отваря нови възможности за генеративен AI. Инференцията е само първата стъпка; тези модели могат да се използват за различни задачи в среди с ограничени ресурси, изисквания за ниска латентност и ограничени разходи.

## **Отключване на Генеративен AI с Phi-3-mini: Ръководство за инференция и внедряване**  
Научете как да използвате Semantic Kernel, Ollama/LlamaEdge и ONNX Runtime, за да получите достъп до и да извършвате инференция с моделите Phi-3-mini, и изследвайте възможностите на генеративния AI в различни приложения.

**Характеристики**  
Инференция на модела Phi-3-mini в:

- [Semantic Kernel](https://github.com/Azure-Samples/Phi-3MiniSamples/tree/main/semantickernel?WT.mc_id=aiml-138114-kinfeylo)  
- [Ollama](https://github.com/Azure-Samples/Phi-3MiniSamples/tree/main/ollama?WT.mc_id=aiml-138114-kinfeylo)  
- [LlamaEdge WASM](https://github.com/Azure-Samples/Phi-3MiniSamples/tree/main/wasm?WT.mc_id=aiml-138114-kinfeylo)  
- [ONNX Runtime](https://github.com/Azure-Samples/Phi-3MiniSamples/tree/main/onnx?WT.mc_id=aiml-138114-kinfeylo)  
- [iOS](https://github.com/Azure-Samples/Phi-3MiniSamples/tree/main/ios?WT.mc_id=aiml-138114-kinfeylo)  

В обобщение, Phi-3-mini позволява на разработчиците да изследват различни формати на модела и да използват генеративен AI в различни сценарии на приложения.

**Отказ от отговорност**:  
Този документ е преведен с помощта на услуги за машинен превод с изкуствен интелект. Въпреки че се стремим към точност, моля, имайте предвид, че автоматичните преводи може да съдържат грешки или неточности. Оригиналният документ на неговия изходен език трябва да се счита за авторитетен източник. За критична информация се препоръчва професионален превод от човек. Не носим отговорност за каквито и да било недоразумения или погрешни интерпретации, произтичащи от използването на този превод.