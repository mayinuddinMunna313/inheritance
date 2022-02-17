# Inheritance

একটি Class অন্য একটি Class থেকে তার properties এবং characteristics বা বৈশিষ্ট্য নেওয়াকে প্রোগ্রামিং ভাষায় Inheritance বলে।

ধরেন Student নামে একটা Base class আছে। Roll ও Name অবশ্যই প্রতি স্টুডেন্ট এর থাকবে। তার মানে এটা তাদের কমন বৈশিষ্ট্য।
class Student {
private int Roll;
protected String Name;
}
এখন Result নামে নতুন আরেকটি ক্লাস নিয়ে এবং এটিকে ডিরাইভড ক্লাস বা ইনহেরিটেড ক্লাস হিসেবে আনি ।
Class Result extends Student
{
private float Mark;
public void Display();
}
এখানে দেখুন Result ক্লাস টি Student ক্লাস কে এক্সটেন্ড করছে । মানে Student ক্লাস যদি বাবা হয় সেই বাবার বৈশিষ্ট্যগুলো চাইল্ড Result ক্লাসের মধ্যে আছে। অর্থাৎ, Student ক্লাসের মধ্যে Roll এবং Name যে দুইটা বৈশিষ্ট্য ছিল সে বৈশিষ্ট্যগুলো Result এর মধ্যে চলে এসেছে। কিন্তু Roll বৈশিষ্ট্য প্রাইভেট হওয়ার কারণে ছেলে, মানে রেজাল্ট ক্লাস এ বৈশিষ্ট্য পাবেনা সরাসরি।
মেম্বারগুলো কিভাবে ইনহেরিটেন্স প্রক্রিয়ায় Result ক্লাসে এসেছে তা যদি দেখাই।
Class Result
{
protected String Name; // Inherited from Student class
private float Mark;
public void Display();
}
