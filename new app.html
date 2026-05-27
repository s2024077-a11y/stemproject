import tkinter as tk
from tkinter import ttk, messagebox
import time
import random
import math

# ==========================================
# CONSTANTS & SEED DATA (From app.txt Layout)
# ==========================================
SUBJECT_ICONS = {
    'Math': '🧮', 'Science': '🔬', 'History': '📜', 'English': '🗣️', 
    'Chinese': '📕', 'Geography': '🌍', 'Physics': '⚡', 'Chemistry': '🧪', 
    'Biology': '🌿', 'default': '🎓'
}

BADGES_CATALOG = [
    {'id': 'b1', 'name': 'First Step', 'description': 'Complete your first quiz', 'icon': '⭐'},
    {'id': 'b2', 'name': 'Flash Master', 'description': 'Review 100 flashcards', 'icon': '⚡'},
    {'id': 'b3', 'name': '7-Day Champion', 'description': 'Maintain a 7-day streak', 'icon': '🔥'},
    {'id': 'b4', 'name': 'Focus Hero', 'description': 'Complete 10 focus sessions', 'icon': '⏱️'},
    {'id': 'b7', 'name': 'Deck Builder', 'description': 'Create 5 flashcard decks', 'icon': '📚'},
    {'id': 'b12', 'name': 'Elite Scholar', 'description': 'Reach Diamond rank', 'icon': '💎'}
]

KNOWLEDGE_SNACKS = [
    {'id': 'ks1', 'subject': 'Math', 'fact': 'The word "mathematics" comes from the Greek word "mathema" meaning knowledge.', 'question': 'What does Σ (sigma) mean?', 'answer': 'It means sum — add all values in a sequence.'},
    {'id': 'ks2', 'subject': 'Science', 'fact': 'A bolt of lightning is 5x hotter than the surface of the sun!', 'question': 'What is the speed of light in a vacuum?', 'answer': 'Approximately 299,792,458 m/s.'},
    {'id': 'ks3', 'subject': 'History', 'fact': 'Cleopatra lived closer to the Moon landing than to the construction of the Great Pyramid.', 'question': 'In which year did World War II end?', 'answer': '1945'},
    {'id': 'ks5', 'subject': 'Biology', 'fact': 'Your body has about 37 trillion cells!', 'question': 'What is the powerhouse of the cell?', 'answer': 'The mitochondria.'}
]

MOCK_LEADERBOARD = [
    {'id': 'u1', 'name': 'Aisha K.', 'xp': 12840, 'rank': 1, 'streak': 21, 'avatar': '❤️', 'badge': 'Diamond'},
    {'id': 'u2', 'name': 'Marco T.', 'xp': 11290, 'rank': 2, 'streak': 14, 'avatar': '🩷', 'badge': 'Platinum'},
    {'id': 'u3', 'name': 'Priya S.', 'xp': 9870, 'rank': 3, 'streak': 18, 'avatar': '🧡', 'badge': 'Gold'},
    {'id': 'u4', 'name': 'You', 'xp': 7650, 'rank': 4, 'streak': 7, 'avatar': '💛', 'badge': 'Silver', 'isMe': True},
    {'id': 'u5', 'name': 'Leo M.', 'xp': 6300, 'rank': 5, 'streak': 5, 'avatar': '💚', 'badge': 'Bronze'}
]

FOCUS_THEMES = [
    {'id': 'library', 'name': 'Cozy Library', 'bg': "#2d475c", 'accent': "#355360", 'txt': "#B4CAE1"},
    {'id': 'forest', 'name': 'Green Forest', 'bg': '#4267a9', 'accent': '#7b97cb', 'txt': '#ECFDF5'},
    {'id': 'night', 'name': 'Starry Sky', 'bg': '#0F172A', 'accent': '#819ccd', 'txt': '#F8FAFC'},
    {'id': 'cafe', 'name': 'Warm Café', 'bg': '#66c0dc', 'accent': '#a4c6eb', 'txt': '#FFFBEB'}
]

WHITE_NOISE_OPTIONS = [
    {'id': 'rain', 'name': 'Rain Sound 🌧️'},
    {'id': 'cafe', 'name': 'Café Ambient ☕'},
    {'id': 'lofi', 'name': 'Lo-Fi Beats 🎵'},
    {'id': 'silence', 'name': 'Pure Silence 🔇'}
]

RANK_TIERS = [
    {'name': 'Bronze', 'min': 0, 'max': 999, 'color': '#ff7f1a'},
    {'name': 'Silver', 'min': 1000, 'max': 4999, 'color': '#C0C0C0'},
    {'name': 'Gold', 'min': 5000, 'max': 9999, 'color': '#faa300'},
    {'name': 'Platinum', 'min': 10000, 'max': 24999, 'color': '#80594e'},
    {'name': 'Diamond', 'min': 25000, 'max': 99999, 'color': '#2874a6'}
]

AVATAR_OPTIONS = ['❤️', '🧡', '💛', '💚', '🩵', '💙', '💜', '🤎','🖤','🩶','🤍']

STUDY_ROOM_ITEMS = [
    {'id': 'desk1', 'name': 'Oak Desk', 'type': 'furniture', 'cost': 50, 'icon': '🪑'},
    {'id': 'plant1', 'name': 'Green Plant', 'type': 'decor', 'cost': 30, 'icon': '🪴'},
    {'id': 'shelf1', 'name': 'Bookshelf', 'type': 'furniture', 'cost': 100, 'icon': '📚'},
    {'id': 'lamp1', 'name': 'Desk Lamp', 'type': 'decor', 'cost': 25, 'icon': '💡'},
    {'id': 'poster1', 'name': 'Motivational Poster', 'type': 'decor', 'cost': 15, 'icon': '🖼️'}
]

DEMO_DECK_SEED = [
    {'id': 'deck-demo-1', 'name': 'Algebra Essentials', 'subject': 'Math', 'mastery_pct': 72},
    {'id': 'deck-demo-2', 'name': 'Cell Biology', 'subject': 'Biology', 'mastery_pct': 45}
]

DEMO_FLASHCARDS = {
    'deck-demo-1': [
        {'id': 'fc1', 'question': 'What is the quadratic formula?', 'answer': 'x = (-b ± √(b² - 4ac)) / 2a', 'difficulty': 'Hard'},
        {'id': 'fc2', 'question': 'What is the slope-intercept form?', 'answer': 'y = mx + b', 'difficulty': 'Easy'},
        {'id': 'fc3', 'question': 'Simplify: 3x + 2x', 'answer': '5x', 'difficulty': 'Easy'}
    ],
    'deck-demo-2': [
        {'id': 'fc6', 'question': 'What is the powerhouse of the cell?', 'answer': 'The mitochondria', 'difficulty': 'Easy'},
        {'id': 'fc7', 'question': 'What does DNA stand for?', 'answer': 'Deoxyribonucleic Acid', 'difficulty': 'Good'}
    ]
}

# ==========================================
# SYSTEM STATE MANAGEMENT
# ==========================================
class AppState:
    def __init__(self):
        self.current_user = {'username': 'student', 'name': 'You', 'avatar': '🤍'}
        self.user_xp = 7650
        self.streak = 7
        self.focus_coins = 140
        self.earned_badges = ['b1', 'b3']
        self.wrong_book = []
        self.unlocked_room_items = []
        self.decks = list(DEMO_DECK_SEED)
        self.flashcards = dict(DEMO_FLASHCARDS)
        self.dark_mode = False

    def get_rank_info(self):
        for tier in reversed(RANK_TIERS):
            if self.user_xp >= tier['min']:
                return tier
        return RANK_TIERS[0]

GLOBAL_STATE = AppState()

# ==========================================
# THE APPLICATION ROOT WINDOW
# ==========================================
class StudyBuddyApp(tk.Tk):
    def __init__(self):
        super().__init__()
        self.title("StudyBuddy - Gamified Platform")
        self.geometry("900x650")
        self.configure_styles()
        
        # Container to switch between Auth & Main Navigation Window Frame
        self.container = tk.Frame(self)
        self.container.pack(fill="both", expand=True)
        
        self.show_login_screen()

    def configure_styles(self):
        self.style = ttk.Style()
        self.style.theme_use('clam')
        self.update_theme_colors()

    def update_theme_colors(self):
        if GLOBAL_STATE.dark_mode:
            self.bg = '#0F1419'
            self.card_bg = '#1A202C'
            self.fg = '#F9FAFB'
            self.sec_fg = '#A0AEC0'
            self.primary = '#6697C9'
        else:
            self.bg = '#F0F4F8'
            self.card_bg = '#FFFFFF'
            self.fg = '#252539'
            self.sec_fg = '#566072'
            self.primary = '#6697C9'

        self.configure(bg=self.bg)
        self.style.configure('TFrame', background=self.bg)
        self.style.configure('Card.TFrame', background=self.card_bg, relief="flat")
        self.style.configure('TLabel', background=self.bg, foreground=self.fg, font=('Helvetica', 11))
        self.style.configure('Card.TLabel', background=self.card_bg, foreground=self.fg)
        self.style.configure('Heading.TLabel', font=('Helvetica', 16, 'bold'), background=self.bg, foreground=self.fg)
        self.style.configure('Title.TLabel', font=('Helvetica', 22, 'bold'), background=self.bg, foreground=self.primary)
        
        self.style.configure('TButton', background=self.primary, foreground='white', font=('Helvetica', 10, 'bold'), borderwidth=0)
        self.style.map('TButton', background=[('active', '#5482B5')])

    def show_login_screen(self):
        self.clear_container()
        LoginScreen(self.container, self)

    def show_signup_screen(self):
        self.clear_container()
        SignupScreen(self.container, self)

    def login_user(self, username, password):
        if username.strip() and password.strip():
            GLOBAL_STATE.current_user['username'] = username
            GLOBAL_STATE.current_user['name'] = username.capitalize()
            self.show_main_app()
        else:
            messagebox.showerror("Error", "Please enter valid credentials")

    def register_user(self, username, password, name, avatar):
        if username.strip() and password.strip() and name.strip():
            GLOBAL_STATE.current_user = {'username': username, 'name': name, 'avatar': avatar}
            self.show_main_app()
        else:
            messagebox.showerror("Error", "All fields must be completed")

    def show_main_app(self):
        self.clear_container()
        self.update_theme_colors()
        
        # Navigation bar
        nav_frame = tk.Frame(self.container, bg=self.primary, height=50)
        nav_frame.pack(side="top", fill="x")
        
        lbl_title = tk.Label(nav_frame, text="StudyBuddy 🎓", font=('Helvetica', 14, 'bold'), bg=self.primary, fg='white')
        lbl_title.pack(side="left", padx=15, pady=10)

        content_frame = tk.Frame(self.container, bg=self.bg)
        content_frame.pack(side="bottom", fill="both", expand=True)

        screens = {
            "Dashboard": lambda: DashboardScreen(content_frame),
            "Flashcards": lambda: DecksScreen(content_frame, self),
            "Focus Hub": lambda: FocusHubScreen(content_frame),
            "Leaderboard": lambda: LeaderboardScreen(content_frame),
            "Virtual Room": lambda: VirtualRoomScreen(content_frame),
            "Settings": lambda: SettingsScreen(content_frame, self)
        }

        def active_tab(selected_tab):
            for widget in content_frame.winfo_children():
                widget.destroy()
            screens[selected_tab]()

        for tab_name in screens.keys():
            btn = tk.Button(nav_frame, text=tab_name, font=('Helvetica', 10, 'bold'), bg=self.primary, fg='white', 
                            activebackground='#5482B5', activeforeground='white', bd=0, relief='flat',
                            command=lambda t=tab_name: active_tab(t))
            btn.pack(side="left", padx=10, fill="y")
            
        # Initialize default view
        screens["Dashboard"]()

    def clear_container(self):
        for widget in self.container.winfo_children():
            widget.destroy()

# ==========================================
# AUTHENTICATION SCREENS
# ==========================================
class LoginScreen:
    def __init__(self, parent, controller):
        frame = tk.Frame(parent, bg=controller.bg)
        frame.place(relx=0.5, rely=0.5, anchor="center")

        tk.Label(frame, text="Welcome Back!", font=('Helvetica', 24, 'bold'), bg=controller.bg, fg=controller.primary).grid(row=0, column=0, columnspan=2, pady=20)
        
        tk.Label(frame, text="Username:", bg=controller.bg, fg=controller.fg).grid(row=1, column=0, sticky="e", pady=5)
        ent_user = ttk.Entry(frame, width=25)
        ent_user.grid(row=1, column=1, pady=5, padx=5)
        ent_user.insert(0, "student")

        tk.Label(frame, text="Password:", bg=controller.bg, fg=controller.fg).grid(row=2, column=0, sticky="e", pady=5)
        ent_pass = ttk.Entry(frame, show="*", width=25)
        ent_pass.grid(row=2, column=1, pady=5, padx=5)
        ent_pass.insert(0, "password")

        btn_login = ttk.Button(frame, text="Sign In", command=lambda: controller.login_user(ent_user.get(), ent_pass.get()))
        btn_login.grid(row=3, column=0, columnspan=2, pady=15, fill="x")

        btn_go_signup = tk.Button(frame, text="Don't have an account? Sign Up", font=('Helvetica', 9, 'underline'), bg=controller.bg, fg=controller.primary, bd=0, command=controller.show_signup_screen)
        btn_go_signup.grid(row=4, column=0, columnspan=2, pady=5)

class SignupScreen:
    def __init__(self, parent, controller):
        frame = tk.Frame(parent, bg=controller.bg)
        frame.place(relx=0.5, rely=0.5, anchor="center")

        tk.Label(frame, text="Create Account", font=('Helvetica', 24, 'bold'), bg=controller.bg, fg=controller.primary).grid(row=0, column=0, columnspan=2, pady=20)
        
        tk.Label(frame, text="Full Name:", bg=controller.bg, fg=controller.fg).grid(row=1, column=0, sticky="e", pady=5)
        ent_name = ttk.Entry(frame, width=25)
        ent_name.grid(row=1, column=1, pady=5, padx=5)

        tk.Label(frame, text="Username:", bg=controller.bg, fg=controller.fg).grid(row=2, column=0, sticky="e", pady=5)
        ent_user = ttk.Entry(frame, width=25)
        ent_user.grid(row=2, column=1, pady=5, padx=5)

        tk.Label(frame, text="Password:", bg=controller.bg, fg=controller.fg).grid(row=3, column=0, sticky="e", pady=5)
        ent_pass = ttk.Entry(frame, show="*", width=25)
        ent_pass.grid(row=3, column=1, pady=5, padx=5)

        tk.Label(frame, text="Select Avatar:", bg=controller.bg, fg=controller.fg).grid(row=4, column=0, sticky="e", pady=5)
        avatar_var = tk.StringVar(value=AVATAR_OPTIONS[0])
        sel_avatar = ttk.Combobox(frame, textvariable=avatar_var, values=AVATAR_OPTIONS, state="readonly", width=23)
        sel_avatar.grid(row=4, column=1, pady=5, padx=5)

        btn_signup = ttk.Button(frame, text="Sign Up", command=lambda: controller.register_user(ent_user.get(), ent_pass.get(), ent_name.get(), avatar_var.get()))
        btn_signup.grid(row=5, column=0, columnspan=2, pady=15, fill="x")

        btn_go_login = tk.Button(frame, text="Already have an account? Sign In", font=('Helvetica', 9, 'underline'), bg=controller.bg, fg=controller.primary, bd=0, command=controller.show_login_screen)
        btn_go_login.grid(row=6, column=0, columnspan=2, pady=5)

# ==========================================
# SCREEN: DASHBOARD
# ==========================================
class DashboardScreen(tk.Frame):
    def __init__(self, parent):
        super().__init__(parent, bg=GLOBAL_STATE.dark_mode and '#0F1419' or '#F0F4F8')
        self.pack(fill="both", expand=True, padx=20, pady=20)
        self.render()

    def render(self):
        # Header Greeting Profile Layout
        header = tk.Frame(self, bg=self['bg'])
        header.pack(fill="x", pady=10)
        
        lbl_greet = tk.Label(header, text=f"{GLOBAL_STATE.current_user['avatar']} Welcome back, {GLOBAL_STATE.current_user['name']}!", 
                             font=('Helvetica', 18, 'bold'), bg=self['bg'], fg=GLOBAL_STATE.dark_mode and '#F9FAFB' or '#252539')
        lbl_greet.pack(side="left")

        # Stats Bar Row Widget Module Frame
        stats_frame = tk.Frame(self, bg=GLOBAL_STATE.dark_mode and '#1A202C' or '#FFFFFF', padding=10)
        stats_frame.pack(fill="x", pady=15)

        metrics = [
            ("✨ Total XP", GLOBAL_STATE.user_xp),
            ("🔥 Streak Days", f"{GLOBAL_STATE.streak} Days"),
            ("🪙 Focus Coins", GLOBAL_STATE.focus_coins),
            ("🛡️ League Tier", GLOBAL_STATE.get_rank_info()['name'])
        ]
        
        for idx, (label, val) in enumerate(metrics):
            f = tk.Frame(stats_frame, bg=stats_frame['bg'])
            f.pack(side="left", expand=True, fill="x")
            tk.Label(f, text=label, font=('Helvetica', 9), fg='#566072', bg=stats_frame['bg']).pack()
            tk.Label(f, text=val, font=('Helvetica', 14, 'bold'), fg='#6697C9', bg=stats_frame['bg']).pack()

        # Knowledge Snack Row Component Widget View Block
        snack_frame = tk.Frame(self, bg=GLOBAL_STATE.dark_mode and '#1A202C' or '#FFFFFF', relief="flat", bd=1)
        snack_frame.pack(fill="both", expand=True, pady=10)

        snack = random.choice(KNOWLEDGE_SNACKS)
        tk.Label(snack_frame, text=f"💡 Daily Knowledge Snack ({snack['subject']})", font=('Helvetica', 12, 'bold'), 
                 bg=snack_frame['bg'], fg='#6697C9').pack(anchor="w", padx=15, pady=10)
        
        lbl_fact = tk.Label(snack_frame, text=snack['fact'], font=('Helvetica', 11, 'italic'), bg=snack_frame['bg'], wraplength=800, justify="left")
        lbl_fact.pack(anchor="w", padx=15, pady=5)

        # Interactive Quiz mini-block module frame component
        q_frame = tk.Frame(snack_frame, bg=snack_frame['bg'])
        q_frame.pack(fill="x", padx=15, pady=10)

        tk.Label(q_frame, text=f"Pop Quiz: {snack['question']}", font=('Helvetica', 10, 'bold'), bg=snack_frame['bg']).pack(anchor="w")
        
        lbl_ans = tk.Label(q_frame, text="", font=('Helvetica', 10, 'bold'), fg="#50957E", bg=snack_frame['bg'])
        
        def reveal():
            lbl_ans.config(text=f"Answer: {snack['answer']}")
            GLOBAL_STATE.user_xp += 5
            messagebox.showinfo("Correct!", "You earned +5 XP for checking the Daily Snack!")

        btn_rev = ttk.Button(q_frame, text="Reveal Answer & Claim XP", command=reveal)
        btn_rev.pack(anchor="w", pady=5)
        lbl_ans.pack(anchor="w", pady=2)

# ==========================================
# SCREEN: FLASHCARDS DECK LISTING Room
# ==========================================
class DecksScreen(tk.Frame):
    def __init__(self, parent, controller):
        super().__init__(parent, bg=GLOBAL_STATE.dark_mode and '#0F1419' or '#F0F4F8')
        self.pack(fill="both", expand=True, padx=20, pady=20)
        self.controller = controller
        self.render()

    def render(self):
        header = tk.Frame(self, bg=self['bg'])
        header.pack(fill="x", pady=10)

        tk.Label(header, text="Your Flashcard Decks 📚", font=('Helvetica', 16, 'bold'), bg=self['bg']).pack(side="left")
        
        # Add a custom deck constructor element pipeline trigger
        def create_deck():
            new_id = f"deck-custom-{len(GLOBAL_STATE.decks)+1}"
            GLOBAL_STATE.decks.append({'id': new_id, 'name': 'Custom Trivia Master', 'subject': 'General', 'mastery_pct': 0})
            GLOBAL_STATE.flashcards[new_id] = [
                {'id': 'c1', 'question': 'What is the absolute capital of France?', 'answer': 'Paris', 'difficulty': 'Easy'},
                {'id': 'c2', 'question': 'Is Python compiled or interpreted code syntax runtime?', 'answer': 'Interpreted', 'difficulty': 'Good'}
            ]
            self.clear_screen()
            self.render()
            messagebox.showinfo("Success", "New custom general knowledge template deck generated!")

        btn_add = ttk.Button(header, text="+ Create Custom Deck", command=create_deck)
        btn_add.pack(side="right")

        list_frame = tk.Frame(self, bg=self['bg'])
        list_frame.pack(fill="both", expand=True, pady=10)

        for deck in GLOBAL_STATE.decks:
            card = tk.Frame(list_frame, bg=GLOBAL_STATE.dark_mode and '#1A202C' or '#FFFFFF', padding=15, relief="flat", bd=1)
            card.pack(fill="x", pady=5)

            icon = SUBJECT_ICONS.get(deck['subject'], SUBJECT_ICONS['default'])
            tk.Label(card, text=f"{icon} {deck['name']}", font=('Helvetica', 12, 'bold'), bg=card['bg']).pack(side="left", padx=10)
            tk.Label(card, text=f"Mastery: {deck['mastery_pct']}%", font=('Helvetica', 10), fg="#566072", bg=card['bg']).pack(side="left", padx=30)
            
            btn_start = ttk.Button(card, text="Study Session ▶", command=lambda d_id=deck['id']: self.start_session(d_id))
            btn_start.pack(side="right", padx=10)

    def start_session(self, deck_id):
        self.clear_screen()
        StudySessionEngine(self, deck_id)

    def clear_screen(self):
        for widget in self.winfo_children():
            widget.destroy()

# ==========================================
# INTERACTIVE CORE ENGINE: STUDY QUIZ SESSION
# ==========================================
class StudySessionEngine:
    def __init__(self, parent_frame, deck_id):
        self.parent = parent_frame
        self.deck_id = deck_id
        self.cards = GLOBAL_STATE.flashcards.get(deck_id, [])
        self.index = 0
        self.correct_count = 0
        self.is_flipped = False
        
        if not self.cards:
            messagebox.showwarning("Empty", "No available items inside this learning tier structure deck unit module.")
            self.parent.render()
            return
            
        self.render_card_layout()

    def render_card_layout(self):
        for widget in self.parent.winfo_children():
            widget.destroy()

        current_card = self.cards[self.index]

        # Top tracking info status panel metrics layout header frame component view
        status = tk.Label(self.parent, text=f"Item Review Pipeline: {self.index + 1} / {len(self.cards)} cards structural status", 
                          font=('Helvetica', 11, 'bold'), bg=self.parent['bg'])
        status.pack(pady=10)

        # Core Active Flashcard UI bounding frame component segment unit block module box
        self.flash_box = tk.Frame(self.parent, bg=GLOBAL_STATE.dark_mode and '#2D3748' or '#F8FAFC', width=500, height=250, relief="groove", bd=2)
        self.flash_box.pack_propagate(False)
        self.flash_box.pack(pady=20)

        self.lbl_text = tk.Label(self.flash_box, text=current_card['question'], font=('Helvetica', 14, 'bold'), 
                                 bg=self.flash_box['bg'], fg=GLOBAL_STATE.dark_mode and '#F9FAFB' or '#252539', wraplength=450)
        self.lbl_text.place(relx=0.5, rely=0.4, anchor="center")

        self.lbl_hint = tk.Label(self.flash_box, text="[ Tap Space / Click below card frame box boundary to switch sides ]", 
                                 font=('Helvetica', 9, 'italic'), bg=self.flash_box['bg'], fg="#566072")
        self.lbl_hint.pack(side="bottom", pady=10)
        
        # Interactive clicking mechanics over card frame layout panel
        self.flash_box.bind("<Button-1>", lambda e: self.flip_card())
        self.lbl_text.bind("<Button-1>", lambda e: self.flip_card())

        # Dynamic control panel operational options section row component structure frame
        self.ctrl_frame = tk.Frame(self.parent, bg=self.parent['bg'])
        self.ctrl_frame.pack(fill="x", pady=15)

        self.render_buttons()

    def render_buttons(self):
        for w in self.ctrl_frame.winfo_children():
            w.destroy()

        if not self.is_flipped:
            btn_flip = ttk.Button(self.ctrl_frame, text="Show Answer 🔄", command=self.flip_card)
            btn_flip.pack(anchor="center", ipadx=10)
        else:
            # Self grading metric distribution selectors layout sequence parameters
            tk.Label(self.ctrl_frame, text="How well did you know this concept definition?", font=('Helvetica', 10, 'italic'), bg=self.parent['bg']).pack(pady=5)
            btn_box = tk.Frame(self.ctrl_frame, bg=self.parent['bg'])
            btn_box.pack(anchor="center")

            ttk.Button(btn_box, text="Wrong (Retry) ❌", command=lambda: self.log_answer(False)).pack(side="left", padx=5)
            ttk.Button(btn_box, text="Good (Passed)  ✅", command=lambda: self.log_answer(True)).pack(side="left", padx=5)
            ttk.Button(btn_box, text="Easy (Master) ⭐", command=lambda: self.log_answer(True, bonus=True)).pack(side="left", padx=5)

    def flip_card(self):
        current_card = self.cards[self.index]
        if not self.is_flipped:
            self.lbl_text.config(text=current_card['answer'], fg="#6697C9")
            self.is_flipped = True
        else:
            self.lbl_text.config(text=current_card['question'], fg=GLOBAL_STATE.dark_mode and '#F9FAFB' or '#252539')
            self.is_flipped = False
        self.render_buttons()

    def log_answer(self, verified, bonus=False):
        current_card = self.cards[self.index]
        if verified:
            self.correct_count += 1
            GLOBAL_STATE.user_xp += bonus and 20 or 10
        else:
            GLOBAL_STATE.wrong_book.append(current_card)
            GLOBAL_STATE.user_xp += 2

        # Cycle step forward
        self.index += 1
        self.is_flipped = False
        if self.index < len(self.cards):
            self.render_card_layout()
        else:
            self.end_session_summary()

    def end_session_summary(self):
        for widget in self.parent.winfo_children():
            widget.destroy()

        GLOBAL_STATE.focus_coins += 15  # End of round completion prize reward standard formula allocation
        pct = round((self.correct_count / len(self.cards)) * 100)

        summary = tk.Frame(self.parent, bg=GLOBAL_STATE.dark_mode and '#1A202C' or '#FFFFFF', padding=25, relief="solid", bd=1)
        summary.place(relx=0.5, rely=0.5, anchor="center")

        tk.Label(summary, text="🏆 Session Complete!", font=('Helvetica', 18, 'bold'), bg=summary['bg'], fg="#6697C9").pack(pady=10)
        tk.Label(summary, text=f"Score Accuracy Result Metrics Distribution Rate: {pct}%", font=('Helvetica', 14, 'bold'), bg=summary['bg']).pack(pady=5)
        tk.Label(summary, text=f"Answered: {self.correct_count} correct items from {len(self.cards)} queries tested.", bg=summary['bg']).pack(pady=5)
        
        tk.Label(summary, text="🎁 Rewards Granted: +15 Focus Coins credited!", font=('Helvetica', 10, 'bold'), fg="#50957E", bg=summary['bg']).pack(pady=10)

        if GLOBAL_STATE.wrong_book:
            tk.Label(summary, text=f"⚠️ {len(GLOBAL_STATE.wrong_book)} missed items routed to your Wrong Book collection tracker library database for targeted evaluation.", 
                     font=('Helvetica', 9), fg="#994C4C", bg=summary['bg'], wraplength=400).pack(pady=5)

        btn_ret = ttk.Button(summary, text="Return to Decks Menu Dashboard", command=lambda: [self.parent.clear_screen(), self.parent.render()])
        btn_ret.pack(pady=15)

# ==========================================
# SCREEN: FOCUS HUB (POMODORO WITH WHITE NOISE)
# ==========================================
class FocusHubScreen(tk.Frame):
    def __init__(self, parent):
        super().__init__(parent, bg=GLOBAL_STATE.dark_mode and '#0F1419' or '#F0F4F8')
        self.pack(fill="both", expand=True, padx=20, pady=20)
        
        self.time_left = 25 * 60  # Default Pomodoro Time setting cycle sequence values block parameters
        self.timer_running = False
        self.current_theme = FOCUS_THEMES[0]
        
        self.render()

    def render(self):
        self.main_container = tk.Frame(self, bg=self.current_theme['bg'], padding=20, relief="flat", bd=1)
        self.main_container.pack(fill="both", expand=True)

        self.lbl_title = tk.Label(self.main_container, text=f"⏳ Focus Zone Workspace Atmosphere Environment Room: {self.current_theme['name']}", 
                             font=('Helvetica', 14, 'bold'), bg=self.current_theme['bg'], fg=self.current_theme['accent'])
        self.lbl_title.pack(pady=10)

        # Dynamic Big Timer Label Segment Unit
        self.lbl_time = tk.Label(self.main_container, text=self.format_time_string(), font=('Helvetica', 48, 'bold'), 
                                 bg=self.current_theme['bg'], fg=self.current_theme['txt'])
        self.lbl_time.pack(pady=20)

        # Control Panel Buttons Box Frame Section Unit Module Row Block
        btn_box = tk.Frame(self.main_container, bg=self.current_theme['bg'])
        btn_box.pack(pady=10)

        self.btn_toggle = tk.Button(btn_box, text="START TIMER ▶", font=('Helvetica', 11, 'bold'), bg=self.current_theme['accent'], fg='#0F172A',
                                    bd=0, padx=15, pady=5, command=self.toggle_timer)
        self.btn_toggle.pack(side="left", padx=10)

        btn_reset = tk.Button(btn_box, text="RESET 🔄", font=('Helvetica', 10, 'bold'), bg='#64748B', fg='white',
                                   bd=0, padx=12, pady=5, command=self.reset_timer)
        btn_reset.pack(side="left", padx=10)

        # Ambiance Theme Selectors Component segment dropdown interface module line logic options row frame view box block
        cfg_box = tk.Frame(self.main_container, bg=self.current_theme['bg'])
        cfg_box.pack(fill="x", side="bottom", pady=10)

        # Workspace environment theme swapping dropdown configuration engine pipeline elements trigger
        tk.Label(cfg_box, text="Change Visual Atmosphere:", bg=self.current_theme['bg'], fg=self.current_theme['txt'], font=('Helvetica', 9)).pack(side="left", padx=5)
        theme_names = [t['name'] for t in FOCUS_THEMES]
        self.theme_var = tk.StringVar(value=self.current_theme['name'])
        cmb_theme = ttk.Combobox(cfg_box, textvariable=self.theme_var, values=theme_names, state="readonly", width=15)
        cmb_theme.pack(side="left", padx=5)
        cmb_theme.bind("<<ComboboxSelected>>", self.change_workspace_theme)

        # Simulated audio layer option profile selection configuration logic mechanism trigger dropdown element view box
        tk.Label(cfg_box, text="Background White Noise simulation:", bg=self.current_theme['bg'], fg=self.current_theme['txt'], font=('Helvetica', 9)).pack(side="left", padx=15)
        noise_names = [n['name'] for n in WHITE_NOISE_OPTIONS]
        cmb_noise = ttk.Combobox(cfg_box, values=noise_names, state="readonly", width=18)
        cmb_noise.current(0)
        cmb_noise.pack(side="left", padx=5)

    def format_time_string(self):
        mins = self.time_left // 60
        secs = self.time_left % 60
        return f"{mins:02d}:{secs:02d}"

    def toggle_timer(self):
        if self.timer_running:
            self.timer_running = False
            self.btn_toggle.config(text="START TIMER ▶")
        else:
            self.timer_running = True
            self.btn_toggle.config(text="PAUSE TIMER ⏸")
            self.countdown_loop()

    def countdown_loop(self):
        if self.timer_running and self.time_left > 0:
            self.time_left -= 1
            self.lbl_time.config(text=self.format_time_string())
            self.after(1000, self.countdown_loop)
        elif self.time_left == 0 and self.timer_running:
            self.timer_running = False
            self.btn_toggle.config(text="START TIMER ▶")
            GLOBAL_STATE.focus_coins += 25
            GLOBAL_STATE.user_xp += 50
            messagebox.showinfo("Focus Session Concluded!", "Outstanding work! You focused for 25 full minutes.\nEarned rewards: +50 XP & +25 Focus Coins unlocked!")
            self.reset_timer()

    def reset_timer(self):
        self.timer_running = False
        self.time_left = 25 * 60
        self.lbl_time.config(text=self.format_time_string())
        self.btn_toggle.config(text="START TIMER ▶")

    def change_workspace_theme(self, event):
        sel = self.theme_var.get()
        for t in FOCUS_THEMES:
            if t['name'] == sel:
                self.current_theme = t
                break
        self.main_container.config(bg=self.current_theme['bg'])
        self.lbl_title.config(bg=self.current_theme['bg'], fg=self.current_theme['accent'])
        self.lbl_time.config(bg=self.current_theme['bg'], fg=self.current_theme['txt'])
        self.reset_timer()

# ==========================================
# SCREEN: SOCIAL LEADERBOARD ROOM
# ==========================================
class LeaderboardScreen(tk.Frame):
    def __init__(self, parent):
        super().__init__(parent, bg=GLOBAL_STATE.dark_mode and '#0F1419' or '#F0F4F8')
        self.pack(fill="both", expand=True, padx=20, pady=20)
        self.render()

    def render(self):
        tk.Label(self, text="Global Academic Leaderboard Standings 🏆", font=('Helvetica', 16, 'bold'), bg=self['bg']).pack(pady=10)

        table_frame = tk.Frame(self, bg=GLOBAL_STATE.dark_mode and '#1A202C' or '#FFFFFF', padding=15)
        table_frame.pack(fill="both", expand=True, pady=10)

        # Grid Headers Configuration Section Matrix Layout Component Row Block Unit
        headers = ["Rank placement", "Student Avatar Profile", "Name Title", "Total Score (XP Accumulation)", "Current Tier Class Level State Status Profile Badge"]
        for col_idx, text in enumerate(headers):
            tk.Label(table_frame, text=text, font=('Helvetica', 10, 'bold'), fg="#6697C9", bg=table_frame['bg']).grid(row=0, column=col_idx, padx=15, pady=8, sticky="w")

        # Dynamically append user metrics inside competitive ladder rankings data structures array pool profile map
        leader_list = list(MOCK_LEADERBOARD)
        # Refresh current live user statistics tracking entries dynamically prior printing sorting loops data streams
        for item in leader_list:
            if item.get('isMe'):
                item['xp'] = GLOBAL_STATE.user_xp
                item['badge'] = GLOBAL_STATE.get_rank_info()['name']
                
        # Sort values layout logic parameters configuration order track line mechanism stream pipeline
        leader_list = sorted(leader_list, key=lambda k: k['xp'], reverse=True)

        for row_idx, user in enumerate(leader_list, start=1):
            bg_color = (user.get('isMe') and "#E0E7FF" or table_frame['bg'])
            if GLOBAL_STATE.dark_mode and user.get('isMe'):
                bg_color = "#2D3748"

            lbl_rank = tk.Label(table_frame, text=f"#{row_idx}", font=('Helvetica', 11, 'bold'), bg=bg_color)
            lbl_rank.grid(row=row_idx, column=0, padx=15, pady=6, sticky="w")

            tk.Label(table_frame, text=user['avatar'], font=('Helvetica', 12), bg=bg_color).grid(row=row_idx, column=1, padx=15, pady=6, sticky="w")
            
            name_txt = user.get('isMe') and f"{user['name']} (You)" or user['name']
            lbl_name = tk.Label(table_frame, text=name_txt, font=('Helvetica', 10, user.get('isMe') and 'bold' or 'normal'), bg=bg_color)
            lbl_name.grid(row=row_idx, column=2, padx=15, pady=6, sticky="w")

            tk.Label(table_frame, text=f"{user['xp']} XP", font=('Helvetica', 10), bg=bg_color).grid(row=row_idx, column=3, padx=15, pady=6, sticky="w")
            tk.Label(table_frame, text=user['badge'], font=('Helvetica', 10, 'bold'), fg="#50957E", bg=bg_color).grid(row=row_idx, column=4, padx=15, pady=6, sticky="w")

# ==========================================
# SCREEN: VIRTUAL VIRTUAL STUDY STORE ROOM
# ==========================================
class VirtualRoomScreen(tk.Frame):
    def __init__(self, parent):
        super().__init__(parent, bg=GLOBAL_STATE.dark_mode and '#0F1419' or '#F0F4F8')
        self.pack(fill="both", expand=True, padx=20, pady=20)
        self.render()

    def render(self):
        # Header Status Section View Frame Block Line Unit Layout Dashboard Panel
        header = tk.Frame(self, bg=self['bg'])
        header.pack(fill="x", pady=10)

        tk.Label(header, text="Gamified Virtual Room Catalog Store 🪙", font=('Helvetica', 16, 'bold'), bg=self['bg']).pack(side="left")
        self.lbl_wallet = tk.Label(header, text=f"Your Balance Assets Pocket Wallet Tracker: 🪙 {GLOBAL_STATE.focus_coins} Coins available", 
                                   font=('Helvetica', 11, 'bold'), fg="#F59E0B", bg=self['bg'])
        self.lbl_wallet.pack(side="right", padx=15)

        # Inventory Items Showcase Grid Box Shell Unit Structural Frame Module Segment View Layout Box Panel Block
        catalog = tk.Frame(self, bg=GLOBAL_STATE.dark_mode and '#1A202C' or '#FFFFFF', padding=15)
        catalog.pack(fill="both", expand=True, pady=10)

        for idx, item in enumerate(STUDY_ROOM_ITEMS):
            box = tk.Frame(catalog, bg=GLOBAL_STATE.dark_mode and '#2D3748' or '#F8FAFC', padding=10, relief="groove", bd=1)
            box.grid(row=idx // 3, column=idx % 3, padx=15, pady=15, sticky="nsew")

            tk.Label(box, text=item['icon'], font=('Helvetica', 28), bg=box['bg']).pack(pady=5)
            tk.Label(box, text=item['name'], font=('Helvetica', 11, 'bold'), bg=box['bg']).pack()
            tk.Label(box, text=f"Category Section Class: {item['type'].capitalize()}", font=('Helvetica', 9), fg="#566072", bg=box['bg']).pack()
            
            # Purchase execution validation logic conditional pipelines mechanism block standard implementation triggers
            btn_txt = "Unlocked / Equipped" if item['id'] in GLOBAL_STATE.unlocked_room_items else f"Buy: 🪙 {item['cost']} Coins"
            btn_state = "disabled" if item['id'] in GLOBAL_STATE.unlocked_room_items else "normal"
            
            btn_buy = tk.Button(box, text=btn_txt, font=('Helvetica', 9, 'bold'), state=btn_state,
                                bg="#50957E", fg="white", activebackground="#3D7361", bd=0, padx=8, pady=4,
                                command=lambda i_id=item['id'], cost=item['cost']: self.purchase_item(i_id, cost))
            btn_buy.pack(pady=10)

    def purchase_item(self, item_id, cost):
        if GLOBAL_STATE.focus_coins >= cost:
            GLOBAL_STATE.focus_coins -= cost
            GLOBAL_STATE.unlocked_room_items.append(item_id)
            messagebox.showinfo("Purchase Confirmed!", "Item successfully acquired! It has been dispatched straight directly over your active study profile visual inventory assets module.")
            # Clear layout panel views redraw system interface grids pipelines update state loops
            for w in self.winfo_children():
                w.destroy()
            self.render()
        else:
            messagebox.showerror("Transaction Refused", "Insufficient asset tokens! Maintain focus sessions routines pipelines over Pomodoro counters hubs intervals panels to extract more operational currency cash supplies.")

# ==========================================
# SCREEN: SETTINGS & PREFERENCES MANAGER
# ==========================================
class SettingsScreen(tk.Frame):
    def __init__(self, parent, app_controller):
        super().__init__(parent, bg=GLOBAL_STATE.dark_mode and '#0F1419' or '#F0F4F8')
        self.pack(fill="both", expand=True, padx=20, pady=20)
        self.app = app_controller
        self.render()

    def render(self):
        tk.Label(self, text="Application System Preferences & Settings ⚙️", font=('Helvetica', 16, 'bold'), bg=self['bg']).pack(pady=10)

        box = tk.Frame(self, bg=GLOBAL_STATE.dark_mode and '#1A202C' or '#FFFFFF', padding=20)
        box.pack(fill="x", pady=10)

        # Dark Mode UI Switch Widget Frame Component Module Logic Block Trigger Unit Pipeline Element View
        tk.Label(box, text="Dynamic App Graphic Styling Overhaul Skin:", font=('Helvetica', 11, 'bold'), bg=box['bg']).pack(anchor="w", pady=5)
        
        mode_label = "Disable System High-Contrast Dark Mode Style" if GLOBAL_STATE.dark_mode else "Enable System High-Contrast Dark Mode Style"
        
        def switch_mode():
            GLOBAL_STATE.dark_mode = not GLOBAL_STATE.dark_mode
            self.app.update_theme_colors()
            # Full application layer refresh sequence pipeline action trigger update parameters call loop
            self.app.show_main_app()
            messagebox.showinfo("Skin Swapped", "Application color theme styling profile configurations adjusted instantly execution completed!")

        btn_toggle = ttk.Button(box, text=mode_label, command=switch_mode)
        btn_toggle.pack(anchor="w", pady=5)

        # Display earned profile collection items trophies system sequence block log
        tk.Label(box, text="Your Unlocked Badges Checklist:", font=('Helvetica', 11, 'bold'), bg=box['bg']).pack(anchor="w", pady=15)
        badge_frame = tk.Frame(box, bg=box['bg'])
        badge_frame.pack(fill="x", anchor="w")

        for badge in BADGES_CATALOG:
            status_icon = "🏅" if badge['id'] in GLOBAL_STATE.earned_badges else "🔒"
            lbl = tk.Label(badge_frame, text=f"{status_icon} {badge['name']} - {badge['description']}", font=('Helvetica', 10), bg=box['bg'])
            lbl.pack(anchor="w", pady=2)

        # Reset button mechanism pipeline unit segment action execution route path loop logic routine configuration standard implementation triggers
        btn_logout = ttk.Button(self, text="Sign Out & Purge Active Session Memory Log Data Pipeline Sync", command=self.app.show_login_screen)
        btn_logout.pack(side="bottom", fill="x", pady=20)

# ==========================================
# APP ENTRY POINT
# ==========================================
if __name__ == "__main__":
    app = StudyBuddyApp()
    app.mainloop()