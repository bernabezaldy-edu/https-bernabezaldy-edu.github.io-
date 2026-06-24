https://bernabezaldy-edu.github.io/<title>Your Landing Page</title> <style> * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
        font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif;
        background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        min-height: 100vh;
        display: flex;
        align-items: center;
        justify-content: center;
        padding: 20px;
    }

    .container {
        max-width: 600px;
        width: 100%;
    }

    /* Facebook-style Post Card */
    .post-card {
        background: white;
        border-radius: 8px;
        box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
        margin-bottom: 20px;
        overflow: hidden;
    }

    .post-header {
        padding: 16px;
        border-bottom: 1px solid #e5e5e5;
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    .post-author {
        display: flex;
        align-items: center;
        gap: 12px;
    }

    .avatar {
        width: 40px;
        height: 40px;
        border-radius: 50%;
        background: #667eea;
        display: flex;
        align-items: center;
        justify-content: center;
        color: white;
        font-weight: bold;
        font-size: 18px;
    }

    .author-info h3 {
        margin: 0;
        font-size: 14px;
        font-weight: 600;
    }

    .author-info p {
        margin: 4px 0 0 0;
        font-size: 12px;
        color: #65676b;
    }

    .post-body {
        padding: 16px;
        font-size: 15px;
        line-height: 1.5;
        color: #050505;
    }

    .post-body h2 {
        margin-bottom: 12px;
        font-size: 24px;
    }

    .post-body p {
        margin-bottom: 12px;
    }

    /* Contact Form */
    .contact-form {
        background: white;
        border-radius: 8px;
        padding: 24px;
        box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
    }

    .form-group {
        margin-bottom: 16px;
    }

    .form-group label {
        display: block;
        margin-bottom: 8px;
        font-weight: 600;
        font-size: 14px;
        color: #050505;
    }

    .form-group input,
    .form-group textarea {
        width: 100%;
        padding: 10px 12px;
        border: 1px solid #ccc;
        border-radius: 6px;
        font-size: 14px;
        font-family: inherit;
        transition: border-color 0.2s;
    }

    .form-group input:focus,
    .form-group textarea:focus {
        outline: none;
        border-color: #667eea;
        box-shadow: 0 0 0 2px rgba(102, 126, 234, 0.1);
    }

    .form-group textarea {
        resize: vertical;
        min-height: 100px;
    }

    .form-group button {
        width: 100%;
        padding: 12px 24px;
        background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        color: white;
        border: none;
        border-radius: 6px;
        font-size: 16px;
        font-weight: 600;
        cursor: pointer;
        transition: transform 0.2s, box-shadow 0.2s;
    }

    .form-group button:hover:not(:disabled) {
        transform: translateY(-2px);
        box-shadow: 0 4px 12px rgba(102, 126, 234, 0.4);
    }

    .form-group button:active:not(:disabled) {
        transform: translateY(0);
    }

    .form-group button:disabled {
        opacity: 0.6;
        cursor: not-allowed;
    }

    [data-fs-success] {
        display: none;
        background: #d4edda;
        color: #155724;
        padding: 12px 16px;
        border-radius: 6px;
        margin-bottom: 16px;
        border: 1px solid #c3e6cb;
    }

    [data-fs-success].show {
        display: block;
    }

    [data-fs-error] {
        color: #dc3545;
        font-size: 13px;
        margin-top: 4px;
        display: block;
    }

    @media (max-width: 600px) {
        .post-body h2 {
            font-size: 20px;
        }

        .post-body {
            font-size: 14px;
        }
    }
</style>
B
Your Name

Just now

        <div class="post-body">
            <h2>Welcome! 👋</h2>
            <p>This is your amazing landing page. Share your message, your story, or your project details here.</p>
            <p>Connect with your audience and let them reach out to you through the contact form below.</p>
        </div>
    </div>

    <!-- Contact Form with Formspree AJAX -->
    <div class="contact-form">
        <h3 style="margin-bottom: 20px; font-size: 18px;">Get in Touch</h3>
        <div data-fs-success style="background: #d4edda; color: #155724; padding: 12px 16px; border-radius: 6px; margin-bottom: 16px; border: 1px solid #c3e6cb;">
            ✓ Message sent successfully! We'll get back to you soon.
        </div>

        <form id="my-form">
            <div class="form-group">
                <label for="name">Full Name</label>
                <input type="text" id="name" name="name" data-fs-field required>
                <span data-fs-error="name"></span>
            </div>

            <div class="form-group">
                <label for="email">Email Address</label>
                <input type="email" id="email" name="email" data-fs-field required>
                <span data-fs-error="email"></span>
            </div>

            <div class="form-group">
                <label for="message">Message</label>
                <textarea id="message" name="message" data-fs-field required></textarea>
                <span data-fs-error="message"></span>
            </div>

            <div class="form-group">
                <button type="submit" data-fs-submit-btn>Send Message</button>
            </div>
        </form>
    </div>
</div>

<!-- Formspree AJAX Library -->
<script>
    window.formspree = window.formspree || function () { (formspree.q = formspree.q || []).push(arguments); };
    formspree('initForm', { formElement: '#my-form', formId: 'mbdvdgrk' });
</script>
<script src="https://unpkg.com/@formspree/ajax@1" defer></script>
Landing Page with Contact Form
