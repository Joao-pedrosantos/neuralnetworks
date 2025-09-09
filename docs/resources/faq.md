# Frequently Asked Questions

## General Questions

### Q: What prerequisites do I need for this course?
**A:** You should have:
- Basic Python programming knowledge
- Understanding of linear algebra and calculus
- Familiarity with NumPy and Matplotlib
- Basic machine learning concepts

### Q: How long does it take to complete each exercise?
**A:** Time estimates:
- **Exercise 1A**: 30-45 minutes
- **Exercise 1B**: 45-60 minutes  
- **Exercise 1C**: 60-75 minutes

### Q: Can I use Google Colab instead of local Jupyter?
**A:** Yes! All exercises work in Google Colab. Just upload the notebook files to your Google Drive.

## Technical Questions

### Q: I'm getting import errors. What should I do?
**A:** Common solutions:
1. Make sure your environment is activated
2. Install missing packages: `pip install package-name`
3. Restart your Jupyter kernel
4. Check our [Setup Guide](setup.md)

### Q: The plots are not showing in my notebook
**A:** Try adding this magic command at the top of your notebook:
```python
%matplotlib inline
```

### Q: How do I save my progress?
**A:** Jupyter notebooks auto-save, but you can also:
- Use Ctrl+S (Cmd+S on Mac) to save manually
- Export notebooks as PDF or HTML for backup
- Commit changes to your Git repository

## Exercise-Specific Questions

### Q: My generated data looks different from the examples
**A:** This is normal! Random data generation creates different results each time. Use `np.random.seed()` for reproducible results.

### Q: How do I know if my classes are separable?
**A:** Look for:
- Clear visual separation in scatter plots
- Minimal or no overlap between class regions
- Ability to draw a straight line separating classes

### Q: What if I can't complete all the questions?
**A:** Focus on understanding the concepts. You can:
- Skip challenging questions initially
- Return to them after completing other parts
- Ask for help on GitHub Issues

## Course Structure Questions

### Q: Do I need to complete exercises in order?
**A:** Yes, exercises build upon each other. Complete them sequentially for the best learning experience.

### Q: Are there solutions available?
**A:** Solutions are embedded in the notebook exercises. Work through the problems first, then check the provided solutions.

### Q: Can I modify the exercise code?
**A:** Absolutely! Experimentation is encouraged. Try:
- Different parameter values
- Additional visualizations
- Extended analysis

## Getting Help

### Q: Where can I get help if I'm stuck?
**A:** Several options:
1. **GitHub Issues**: Create an issue in the repository
2. **GitHub Discussions**: Ask questions and discuss with peers
3. **Setup Guide**: Review the [Tools & Setup](setup.md) section
4. **Documentation**: Check package documentation (NumPy, Matplotlib, etc.)

### Q: How do I report a bug or error in the materials?
**A:** Please create a GitHub Issue with:
- Description of the problem
- Steps to reproduce
- Your environment details (Python version, OS, etc.)
- Screenshots if applicable

### Q: Can I contribute to the course materials?
**A:** Yes! Contributions are welcome:
- Fix typos or errors
- Suggest improvements
- Add additional examples
- Create pull requests with your changes

## Academic Questions

### Q: Can I use this course for academic credit?
**A:** This depends on your institution. The materials are designed for educational use and can supplement formal courses.

### Q: How do I cite this course in my work?
**A:** You can cite it as:
```
Santos, J. P. R. (2025). Artificial Neural Networks and Deep Learning Course. 
GitHub repository: https://github.com/joao-pedrosantos/neuralnetworks
```

### Q: Are there certificates or credentials available?
**A:** This is an open educational resource. No formal certificates are provided, but you'll gain practical skills and knowledge.

## Still Have Questions?

If your question isn't answered here:

1. **Search existing issues** on GitHub
2. **Create a new issue** with the "question" label
3. **Start a discussion** in the GitHub Discussions tab
4. **Check the course documentation** for additional details

We're here to help you succeed! 🎓