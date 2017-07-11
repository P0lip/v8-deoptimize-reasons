# V8 deoptimize reasons

A list of Turbofan+Ignition deoptimize reasons with examples, explanations and advices.

[Your contribution is most welcome!](/CONTRIBUTING.md)
The entire idea of this project originates from [the following project](https://github.com/vhf/v8-bailout-reasons/)

### What this is about

In order to keep this section short and allow people to get to the primary content of this repo faster, here is what it's all about and why you (probably) should care: [Chromium, Chrome, Node.js, V8, Crankshaft and bailout reasons](https://draft.li/blog/2016/01/22/chromium-chrome-v8-crankshaft-bailout-reasons/).

## Index
### [Deoptimize reasons](#deoptimize-reasons-1)


### [References](#references-1)

* [Resources](#resources)
* [All deoptimize reasons](#all-deoptimize-reasons)

## References
### Resources

* [All bailout reasons in Chromium codebase](https://code.google.com/p/chromium/codesearch#chromium/src/v8/src/bailout-reason.h)
* [Bad value context for arguments value](https://gist.github.com/Hypercubed/89808f3051101a1a97f3)
* [I-want-to-optimize-my-JS-application-on-V8 checklist](http://mrale.ph/blog/2011/12/18/v8-optimization-checklist.html)
* [JavaScript: Performance loss on incorrect arguments using](http://techblog.dorogin.com/2015/05/performance-loss-on-incorrect-arguments-using.html)
* [Optimization killers](https://github.com/petkaantonov/bluebird/wiki/Optimization-killers)
* [OptimizationKillers](https://github.com/zhangchiqing/OptimizationKillers)
* [Performance Tips for JavaScript in V8](http://www.html5rocks.com/en/tutorials/speed/v8/)
* [thlorenz/v8-perf](https://github.com/thlorenz/v8-perf/blob/master/compiler.md)
* [A high-level tutorial about tracing deopts points](https://www.netguru.co/blog/tracing-patterns-hinder-performance)

### All deoptimize reasons
*NOTE*: For the latest deopts list, look at `src/deoptimize-reason.h` in the V8 src.

* V(AccessCheck, "Access check needed")
* V(NoReason, "no reason")
* V(ConstantGlobalVariableAssignment, "Constant global variable assignment")
* V(ConversionOverflow, "conversion overflow")
* V(DivisionByZero, "division by zero")
* V(ExpectedHeapNumber, "Expected heap number")
* V(ExpectedSmi, "Expected smi")
* V(ForcedDeoptToRuntime, "Forced deopt to runtime")
* V(Hole, "hole")
* V(InstanceMigrationFailed, "instance migration failed")
* V(InsufficientTypeFeedbackForCall, "Insufficient type feedback for call")
* V(InsufficientTypeFeedbackForCallWithArguments, "Insufficient type feedback for call with arguments")
* V(InsufficientTypeFeedbackForConstruct, "Insufficient type feedback for construct")
* V(FastPathFailed, "Falling off the fast path")
* V(InsufficientTypeFeedbackForCombinedTypeOfBinaryOperation, "Insufficient type feedback for combined type of binary operation")
* V(InsufficientTypeFeedbackForGenericNamedAccess, "Insufficient type feedback for generic named access")
* V(InsufficientTypeFeedbackForGenericKeyedAccess, "Insufficient type feedback for generic keyed access")
* V(InsufficientTypeFeedbackForLHSOfBinaryOperation, "Insufficient type feedback for LHS of binary operation")
* V(InsufficientTypeFeedbackForRHSOfBinaryOperation, "Insufficient type feedback for RHS of binary operation")
* V(KeyIsNegative, "key is negative")
* V(LostPrecision, "lost precision")
* V(LostPrecisionOrNaN, "lost precision or NaN")
* V(MementoFound, "memento found")
* V(MinusZero, "minus zero")
* V(NaN, "NaN")
* V(NegativeKeyEncountered, "Negative key encountered")
* V(NegativeValue, "negative value")
* V(NoCache, "no cache")
* V(NotAHeapNumber, "not a heap number")
* V(NotAHeapNumberUndefined, "not a heap number/undefined")
* V(NotAJavaScriptObject, "not a JavaScript object")
* V(NotANumberOrOddball, "not a Number or Oddball")
* V(NotASmi, "not a Smi")
* V(NotASymbol, "not a Symbol")
* V(OutOfBounds, "out of bounds")
* V(OutsideOfRange, "Outside of range")
* V(Overflow, "overflow")
* V(Proxy, "proxy")
* V(ReceiverWasAGlobalObject, "receiver was a global object")
* V(Smi, "Smi")
* V(TooManyArguments, "too many arguments")
* V(TracingElementsTransitions, "Tracing elements transitions")
* V(TypeMismatchBetweenFeedbackAndConstant, "Type mismatch between feedback and constant")
* V(UnexpectedCellContentsInConstantGlobalStore, "Unexpected cell contents in constant global store")
* V(UnexpectedCellContentsInGlobalStore, "Unexpected cell contents in global store")
* V(UnexpectedObject, "unexpected object")
* V(UnexpectedRHSOfBinaryOperation, "Unexpected RHS of binary operation")
* V(UnknownMapInPolymorphicAccess, "Unknown map in polymorphic access")
* V(UnknownMapInPolymorphicCall, "Unknown map in polymorphic call")
* V(UnknownMapInPolymorphicElementAccess, "Unknown map in polymorphic element access")
* V(UnknownMap, "Unknown map")
* V(ValueMismatch, "value mismatch")
* V(WrongInstanceType, "wrong instance type")
* V(WrongMap, "wrong map")
* V(UndefinedOrNullInForIn, "null or undefined in for-in")
* V(UndefinedOrNullInToObject, "null or undefined in ToObject")
