<template>
    <footer class="footer">
        <div class="footer-content">
            <div class="footer-links">
                <a href="/feedback" class="footer-link">Feedback</a>
                <a href="https://discord.gg/Fpbg8MpKnm" class="footer-link"
                    >Discord</a
                >
                <a href="/map-creator" class="footer-link">Map Creator</a>
                <a href="https://thunderstore.io/c/bopl-battle/p/MapMakerTeam/Map_Loader/" class="footer-link">Map Loader</a>
                <a href="/docs/" class="footer-link">Wiki</a>
                <a href="/docs/credits/" class="footer-link">Credits</a>
            </div>
            <div class="footer-credit">
                <span>&copy; 2024 Bopl Map Database. All rights reserved.</span>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'FooterComponent',
};
</script>

<style scoped>
.footer {
    margin-top: 20px;
    background-color: var(--bgcol4);
    padding: 20px 0;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    margin-top: auto;
}

.footer-content {
    width: 100%;
    max-width: 1200px;
    text-align: center;
}

.footer-links {
    display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
    margin-bottom: 10px;
}

.footer-link {
    text-decoration: none;
    color: var(--textcol);
    font-size: 16px;
    font-weight: 500;
    transition: color 0.3s;
}

.footer-link:hover {
    color: var(--accent);
}

.footer-credit {
    color: var(--textcol);
    font-size: 14px;
    margin-top: 10px;
}

@media (max-width: 768px) {
    .footer-links {
        flex-direction: row;
        align-items: center;
        gap: 10px;
    }

    .footer-link {
        font-size: 14px;
    }
}
</style>
